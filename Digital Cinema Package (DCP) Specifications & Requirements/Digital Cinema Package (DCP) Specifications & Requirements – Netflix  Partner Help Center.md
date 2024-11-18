> 本文由 [简悦 SimpRead](http://ksria.com/simpread/) 转码， 原文地址 [partnerhelp.netflixstudios.com](https://partnerhelp.netflixstudios.com/hc/en-us/articles/4417542010387-Digital-Cinema-Package-DCP-Specifications-Requirements)

> Skip to Translations Introduction This document outlines specifications and requirements when authori......

[_**Skip to Translations**_](#h_01FX6H1P88QYQGARQQKT9QP1WH)

### **Introduction**

This document outlines specifications and requirements when authoring **Digital Cinema Packages (DCP)** for Netflix. For best practices for DCP see [Digital Cinema Package (DCP): Best Practices](https://partnerhelp.netflixstudios.com/hc/en-us/articles/4417535063955)[.](https://partnerhelp.netflixstudios.com/hc/en-us/articles/4417535063955)

* * *

### **Standard**

Interop (IOP) standard must be used, except in the scenarios described below where SMPTE standard is required.

SMPTE standard must be used for:

*   High Frame Rate (HFR)
*   Dolby ATMOS
*   HDR/Dolby Vision

### **SMPTE Features**

The SMPTE standard has a number of features; however, not all features must be utilized when authoring a SMPTE DCP composition.  The guidelines for SMPTE features for each use case are detailed below:

**High Frame Rate DCP compositions:**

*   must be SMPTE standard.
*   must not include the “CompositionMetadataAsset” (_described in SMPTE ST 429-16_).
*   must not use audio MXF MCA sub descriptor label ULs.

**Dolby ATMOS DCP compositions:**

*   must be SMPTE standard.
*   must be a fully flattened OV DCP composition, with all Subtitles or Open Caption burned-in to the video MXF.
*   must not include the “CompositionMetadataAsset” (_described in SMPTE ST 429-16_).
*   must not use audio MXF MCA sub descriptor label ULs.

**HDR/Dolby Vision DCP compositions:**

*   must be SMPTE standard.
*   must not use audio MXF MCA sub descriptor label ULs.
*   must include the “CompositionMetadataAsset” (_described in SMPTE ST 429-16_) and it must be filled out as completely as possible.
*   the CPL must include the following Extension information in the “ExtensionMetadataList” in the “CompositionMetadataAsset:”

```
<cpl-meta:ExtensionMetadata scope="http://www.dolby.com/schemas/2014/EDRMetadata">
     <cpl-meta:Name>Dolby Vision</cpl-meta:Name>
     <cpl-meta:PropertyList>
          <cpl-meta:Property>
               <cpl-meta:Name>image transfer function</cpl-meta:Name>
               <cpl-meta:Value>PQ10K</cpl-meta:Value>
          </cpl-meta:Property>
     </cpl-meta:PropertyList>
</cpl-meta:ExtensionMetadata>



```

SMPTE features other than those detailed above (_e.g. Markers, Ratings, 3D Subtitles, encrypted Timed Text MXF_) must not be used for High-Frame-Rate, Dolby ATMOS or HDR/Dolby Vision DCP compositions.

### **Reels/Segments**

DCP compositions must be formatted in reels/segments of (22) minutes or less, conformed together seamlessly to represent the long-play form of the content.

The first frame in the first reel/segment in a DCP composition must begin on black, and the last frame in the last reel/segment in a DCP composition must end on black.  This will be accomplished inherently for DCP compositions containing Netflix Theatrical Idents before and after the program (_as the Idents begin and end on black_).

### **Dimension**

DCP compositions must be 2D.

### **Compression Rates**

The image must be encoded to DCI specification JPEG-2000 with a maximum Variable Bitrate (VBR) of 250MB/s, or 500Mb/s for HDR/Dolby Vision and High Frame Rate content.

Some authoring partners choose to limit the maximum bitrate to 245MB/s for Standard-Dynamic-Range (SDR) content to prevent the possibility of the bitrate spiking above 250MB/s.  This is an acceptable practice.

### **Resolution & Aspect Ratio**

DCP compositions must be DCI 4K container resolution, either 3996x2160 (1.85/Flat) or 4096x1716 (2.39/Scope).

With prior approval by Netflix, a DCI 2K container resolution may be used, either 1998x1080 (1.85/Flat) or 2048x858 (2.39 Scope).

Content with a 1.85 aspect ratio or 2.39 aspect ratio must utilize the full container resolution (_DCI Flat or DCI Scope respectively_), the image must fill the frame, edge-to-edge vertically and horizontally.

All other resolutions must be sized and ‘padded’ with black to fill a DCI Flat or DCI Scope container resolution.  

If the content has an aspect ratio of less than 2.30 (_e.g. 2.00, 1.89, 1.78, 1.66, 1.33_) the active image must be fit to a DCI Flat container.

If the content has an aspect ratio equal to or greater than 2.30 (_e.g. 2.35, 2.50_) the active image must be fit to a DCI Scope container.

In these scenarios, fit the active picture to the container resolution, aligning with either the top and bottom edge or left and right edge, as appropriate for the aspect ratio.  A pillarboxed or letterboxed image is expected in these scenarios.  

Do not crop or ‘blow-up’ the image to fill the container.

### **Frame Rates**

If the native frame rate of the source content is not true-24fps, consult with your Netflix representative to confirm the frame rate desired for the DCP composition.

For Interop (IOP) standard DCP compositions, the frame rate must be 24fps.

For SMPTE standard DCP compositions, the frame rate may be 24fps, 25fps or 30fps for 2K or 4K, and may be 48fps, 50fps or 60fps for 2K.  

### **Audio Configuration**

Audio MXF files must always have an even number of tracks (_i.e. divisible by 2_).

Audio MXF must have either (8) or (16) channels, with unused channels containing silence/MOS.

For SMPTE standard DCP compositions, the audio MXF must use the “Configuration 4” Channel Assignment UL (_per SMPTE ST 4290-2_), commonly referred to as “Wild Track Format.”  No other channel formats (_including “Undefined” or “0”_) must be utilized.

<table><tbody><tr><td><p>Channel</p></td><td><p>1</p></td><td><p>2</p></td><td><p>3</p></td><td><p>4</p></td><td><p>5</p></td><td><p>6</p></td><td><p>7</p></td><td><p>8</p></td><td><p>9</p></td><td><p>10</p></td><td><p>11</p></td><td><p>12</p></td><td><p>13</p></td><td><p>14</p></td><td><p>15</p></td><td><p>16</p></td></tr><tr><td><p>5.1</p></td><td><p>L</p></td><td><p>R</p></td><td><p>C</p></td><td><p>LFE</p></td><td><p>Ls</p></td><td><p>Rs</p></td><td><p>-</p></td><td><p>-</p></td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td></tr><tr><td><p>7.1</p></td><td><p>L</p></td><td><p>R</p></td><td><p>C</p></td><td><p>LFE</p></td><td><p>Lss</p></td><td><p>Rss</p></td><td><p>-</p></td><td><p>-</p></td><td><p>-</p></td><td><p>-</p></td><td><p>Lrs</p></td><td><p>Rrs</p></td><td><p>-</p></td><td><p>-</p></td><td><p>-</p></td><td><p>-</p></td></tr><tr><td><p>7.1 ATMOS</p></td><td><p>L</p></td><td><p>R</p></td><td><p>C</p></td><td><p>LFE</p></td><td><p>Lss</p></td><td><p>Rss</p></td><td><p>-</p></td><td><p>-</p></td><td><p>-</p></td><td><p>-</p></td><td><p>Lrs</p></td><td><p>Rrs</p></td><td><p>-</p></td><td><p>Sync</p></td><td><p>-</p></td><td><p>-</p></td></tr></tbody></table>

_The chart above details the MXF audio track layout for 5.1, 7.1 and 7.1-with-ATMOS audio configurations for DCP compositions containing only Print Master audio._

<table><tbody><tr><td><p>Channel</p></td><td><p>1</p></td><td><p>2</p></td><td><p>3</p></td><td><p>4</p></td><td><p>5</p></td><td><p>6</p></td><td><p>7</p></td><td><p>8</p></td><td><p>9</p></td><td><p>10</p></td><td><p>11</p></td><td><p>12</p></td><td><p>13</p></td><td><p>14</p></td><td><p>15</p></td><td><p>16</p></td></tr><tr><td><p>5.1</p></td><td><p>L</p></td><td><p>R</p></td><td><p>C</p></td><td><p>LFE</p></td><td><p>Ls</p></td><td><p>Rs</p></td><td><p>HI</p></td><td><p>VI</p></td><td><p>-</p></td><td><p>-</p></td><td><p>-</p></td><td><p>-</p></td><td><p>DBOX</p></td><td><p>-</p></td><td><p>SLV</p></td><td><p>-</p></td></tr><tr><td><p>7.1</p></td><td><p>L</p></td><td><p>R</p></td><td><p>C</p></td><td><p>LFE</p></td><td><p>Lss</p></td><td><p>Rss</p></td><td><p>HI</p></td><td><p>VI</p></td><td><p>-</p></td><td><p>-</p></td><td><p>Lrs</p></td><td><p>Rrs</p></td><td><p>DBOX</p></td><td><p>-</p></td><td><p>SLV</p></td><td><p>-</p></td></tr><tr><td><p>7.1 ATMOS</p></td><td><p>L</p></td><td><p>R</p></td><td><p>C</p></td><td><p>LFE</p></td><td><p>Lss</p></td><td><p>Rss</p></td><td><p>HI</p></td><td><p>VI</p></td><td><p>-</p></td><td><p>-</p></td><td><p>Lrs</p></td><td><p>Rrs</p></td><td><p>DBOX</p></td><td><p>Sync</p></td><td><p>SLV</p></td><td><p>-</p></td></tr></tbody></table>

_The chart above details the MXF audio track layout for 5.1, 7.1 and 7.1-with-ATMOS audio configurations for DCP compositions that also contain Hearing Impaired (HI) audio, Vision Impaired (VI) audio, D-BOX Motion Control (DBOX) and/or Sign Language Video (SLV)._

### **Timed Text**

Timed Text here refers to Subtitles, Open Captions and Closed Captions.

Language element and attribute code values for Timed Text XML and CPL must conform to ISO RFC 5646.

All Timed Text XML start must always be equal to a value of 00:00:00:00, regardless of the reel/segment number.  There must be no hour-based offsets for reel/segment numbers (_e.g. the reel 2 start value must start at 00:00:00:00, not at 02:00:00:00_).

Font files must not exceed 640kB.

Timed Text XML used for Closed Captions must not exceed 256kB.

PNG image files must be the same resolution and aspect ratio as the intended DCP compositions and must be cropped to fit the exact size of the text.  PNG images must be in RGB colorspace.  

When utilizing PNG image files, the cumulative size limit for each reel/segment must not exceed 115MB.

The “EntryPoint” in a CPL referencing a Timed Text asset must be zero (0).  

The “ReelNumber” in a Timed Text XML must match the corresponding CPL’s reel/segment number.

For Subtitles and Open Captions, the “MainSubtitle” CPL asset type must be used.

Due to playback issues with some equipment, if using both Closed Captions and Subtitles, for every reel/segment that contains one, it must contain the other.

For United States domestic only, the “Language” value within a Closed Caption section of the CPL and the Timed Text header must be “en”.

**For Interop (IOP) standard DCP compositions:**

*   All timed text files and any ancillary files must conform to [“Subtitle Specification (XML File Format) for DLP Cinema Projection Technology” version 1.1.](https://drive.google.com/file/d/1DGEWQPWs6XbbAPresJu4FY6vHFdEXZwk/view?usp=sharing)
*   The same Timed Text XML file must not be reused in different DCP compositions.  In scenarios where a Timed Text XML asset needs to be reused, the “SubtitleID” value must be updated to reflect a new UUID for each instance of the XML.
*   For each reel/segment containing Timed Text, the XML file and all ancillary files (_fonts or PNGs_) must be placed within a subdirectory, and the name of this subdirectory must be the UUID of the XML’s “SubtitleID.”
*   For Closed Captions, the “MainClosedCaption” CPL asset type must be used.
*   The Timed Text XML duration must not be longer than the corresponding reel/segment length.

**For SMPTE standard DCP compositions:**

*   All timed text files and any ancillary files must conform to SMPTE ST 428-7:2014 DCDM Subtitle specification ([_https://www.smpte.org/_](https://www.smpte.org/)).
*   SMPTE Timed Text MXF must not be encrypted.
*   The “IntrinsicDuration” of any Timed Text MXF must be at least the length of the reel it is to be contained in.
*   SMPTE Timed Text XML must use the 2021 XML namespace.
*   The “StartTime” in a Timed Text XML must always be equal to a value of 00:00:00:00, regardless of reel/segment number.
*   For Closed Captions, the “ClosedCaption” CPL asset type must be used.
*   “ClosedSubtitle” or “MainCaption” CPL asset types must not be used.

### **Naming Convention & ‘ContentTitleText’**

The InterSociety Digital Cinema Forum (ISDCF) naming convention (_described at_ [_https://www.isdcf.com/_](https://www.isdcf.com/)) must be used for naming the CPL.

The Netflix “Studio Code” abbreviation is “NET”.

For unencrypted DCP compositions, include "-unenc" as a 'Content Type Modifier' to signify that the DCP composition is unencrypted. (_e.g. Title_FTR-1-unenc_S_EN-XX_US-G_51_4K_NET_20220101_NET_IOP_OV_)

The same naming convention must be used for the “ContentTitleText” value within the CPL.  No two DCP compositions must utilize the exact same “ContentTitleText” value.

The names of individual files within the DCP composition must be as short as possible to avoid path name limitations in the “AssetMap,” but unique enough to avoid file naming collisions when creating DCP compositions containing similarly named files.  

File must consist of alphanumeric characters, hyphens, and/or underscores only: 

[a-z], [ A-Z ], [ 0-9 ], [ _ ], [ - ]

File names must not contain spaces or other special characters.

### **Annotation Text**

Playback and theatre management systems present the “AnnotationText” from either the PKL or CPL at the time the DCP is ingested.

In scenarios where a PKL references a single CPL, the PKL and CPL “AnnotationText” must exactly match the CPL’s “ContentTitleText.”

In scenarios where a PKL references (2) or more CPLs, each CPL’s “Annotation Text” must exactly match that CPL’s “ContentTitleText,” and the primary CPLs “ContentTitleText” must be used for the PKL’s “AnnotationText.”

### **Distribution Key Delivery Messages (DKDM)**

When delivering an encrypted DCP composition to a distribution partner, an active Distribution Key Delivery Message (DKDM) targeted to the leaf certificate for that distribution partner must be provided.

* * *

### **ADDITIONAL REFERENCES**

For additional information, reference these industry standards, specifications and recommended practices:

*   Digital Cinema Initiatives (DCI) System Requirements and Specifications for Digital Cinema [https://www.dcimovies.com](https://www.dcimovies.com/specification/index.html)
*   ISDCF Industry Recommended Practice Technical Documents
*   [https://www.isdcf.com](https://www.isdcf.com/site/technical-docs/)
*   SMPTE DCP Published and Draft Standards 
*   [https://www.smpte.org](https://www.smpte.org/)

Where a topic is unspecified in this document, defer to the above.

* * *

### **CHANGE LOG**

*   **10/19/23**
    *   Removed burned-in subtitle requirements for SMPTE standard DCP compositions containing Dolby Atmos
    *   Moved encryption best practices from this Specifications document to [Digital Cinema Package (DCP): Best Practices](https://partnerhelp.netflixstudios.com/hc/en-us/articles/4417535063955).

**TRANSLATIONS**

**[العربية](https://drive.google.com/file/d/1_BSxQv-p26b4Ww6jIy-4q_vnGA11bha6/view?usp=sharing)**

**[Deutsch](https://drive.google.com/file/d/1-xybon_s_sOlinEGCDbOPLucf79CY3sf/view?usp=sharing)**

**[Español (España)](https://drive.google.com/file/d/198JbYr0uRcn2yQXGnG0QsjR4lsZEV7Hi/view?usp=sharing)**

**[Español (Latinoamérica)](https://drive.google.com/file/d/17Z1zbEmE2uDZq4qE5fiDWm8iaA_lHB6Q/view?usp=sharing)[‬](https://drive.google.com/file/d/1_BSxQv-p26b4Ww6jIy-4q_vnGA11bha6/view?usp=sharing)**

**[Français](https://drive.google.com/file/d/1zDVBnaKpwfNqjssh6jetVciLg5Z1Rhej/view?usp=sharing)**

**[Italiano](https://drive.google.com/file/d/1f2iGhr2DviP7kfHkncxfbNB7Jqv-uOdI/view?usp=sharing)**

**[Polski](https://drive.google.com/file/d/1FoxZB3bO0QmNxgyn5LfWi60N6cj1mJo5/view?usp=sharing)**

**[Português](https://drive.google.com/file/d/17yw6EbdTKChY9Ui4WOg_2BHWOChJwR4z/view?usp=sharing)**

**[日本語](https://drive.google.com/file/d/1tsdS9yIBKBpvNSb1jZUD7akxbRAagg7d/view?usp=sharing)**

**[한국어](https://drive.google.com/file/d/16L_AlTl16KYQICRDM_-CBHu5ewknLM7O/view?usp=sharing)**

**[ไทย](https://drive.google.com/file/d/1_HitXf9reRzY4SVJEj-SMD9W_yCnUzXO/view?usp=sharing)**

**[繁體中文](https://drive.google.com/file/d/1I0KI1j7urejqfTHMyjlrxtTp_kVZH0GW/view?usp=sharing)**

**[Indonesian](https://drive.google.com/file/d/1bK9p11LoiWQp5ShgUOnnY5_4uSdB4Ez1/view?usp=sharing)**

**[русский](https://drive.google.com/file/d/1ZZwe5jTndXpm8yREcfFroOW9esas_rAw/view?usp=sharing)**

**[Türkçe](https://drive.google.com/file/d/1J244KIqn-9poyATdly5ly-InhjgSRWn0/view?usp=sharing)**

Was this article helpful? 2 out of 2 found this helpful