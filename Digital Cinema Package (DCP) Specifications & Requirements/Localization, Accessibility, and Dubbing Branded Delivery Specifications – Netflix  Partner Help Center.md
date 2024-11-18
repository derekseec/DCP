> 本文由 [简悦 SimpRead](http://ksria.com/simpread/) 转码， 原文地址 [partnerhelp.netflixstudios.com](https://partnerhelp.netflixstudios.com/hc/en-us/articles/7357416307603-Localization-Accessibility-and-Dubbing-Branded-Delivery-Specifications#h_01GCD42HQABVDJ9Y3XQQ0HTT9P)

> Version 5.1 Skip to Translations   Welcome Below partners will find delivery specifications required......

_**Version 5.1**_

[Skip to Translations](#h_01GCCWFZCXF0MW1G41BAY7VJVA)

* * *

### **Welcome**

Below partners will find delivery specifications required by Netflix; however, some of them may not apply to your production. Please refer to your Netflix Delivery Requirements List or your Netflix Representative to verify which assets apply to your delivery. 

Enforcement of 5.1 specification changes outlined in the [change log](#h_01HF7XAPYCXV03BPNP4S94CSX7) will begin on January 2nd, 2024.

* * *

### **Table of Contents**

*   [General Asset Requirements](#h_01GCD3YS1H7QDBYYEZV8RJY5NJ)
*   [Subtitle as a Separate File](#h_01GCD3YY4YV3RRNGE84D3QYTT1)
*   [Forced Narrative Subtitles](#h_01GCD3ZHS98GGQ2THAN7NSACW4)
*   [Accessibility Files (SDH)](#h_01GCD3ZR6YWD8N97AFNWEF7HPG)
    *   [SDH as Separate File](#h_01GCD3ZYDV5BX66D631RV8VVVW)
*   [Alternate Language and Audio Description Delivery to Backlot](#h_01GCD408WXJ8HAXEX5YG9Q85B4)
    *   [Acceptable Alternate Language and Audio Description Formats (non-QuickTime)](#h_01GCD40RSCXH9AQBWERNY24KEY)
    *   [Acceptable Alternate Language and Audio Description Formats (QuickTime)](#h_01GCD41MKN260BRKYSFH3RPVEA)
*   [Audio Mix Requirements: Alternate Language and Audio Description](#h_01GCD42902VHTQEJW366F7FT0R)
*   [Dub Cards/Dub Credits](#h_01GCD42HQABVDJ9Y3XQQ0HTT9P)
*   [Appendix](#h_01GCD42T3Q9WNBHBKV8PPAQKYG)
    *   [Language Codes](#h_01GCD42ZXY03986XQZBAZQT83F)

* * *

### **1. General Asset Requirements**

*   Translations within secondary audio and timed text assets should not introduce slurs that were not present in the original language or unnecessarily harshen/soften the language used, unless specifically requested by Netflix.

* * *

### **2. Subtitle as a Separate File**

Subtitles must encompass spoken dialog intended to be understood that differs in language from the subtitle file. Subtitles must also translate any narrative burned-in text that is in a different language from the subtitle file. In the event of overlapping narrative burned-in text and dialog, precedence should be given to the most plot pertinent message.

For example, for an English original language film, the German subtitle file would contain translation for all the non-German dialog spoken.

*   Subtitles must conform, within a half second, to the Primary Video Mezzanine that is delivered or to the Netflix-provided Proxy File. Raster image-based subtitles will not be accepted.
*   Subtitle files must not be censored or contain advertisements, placards, overlay branding, or website link callouts.
*   All subtitle files need to start at hour 00. Netflix does not accept the subtitle timestamps starting at hour 01 or 10, which is common on tape.
*   Include positional data in the subtitle file if the subtitles would otherwise obscure burned-in text.
*   All subtitles must contain an individual credit for the author of the text asset; company credits are not allowed. If more than one translator has worked on an asset, e.g. when translating from multiple source languages or when more than one translator has collaborated on a special project, more than one translator can be mentioned in the same credit.
*   Subtitler credits must be contained to the last event of the file, must not appear before the end of the main program, and must be formatted exactly as they are meant to appear on-screen as required by law in the territory of exhibition.
*   TTML format is required for “Right-to-Left” languages such as Arabic and Hebrew.
*   Translator credits are NOT required for marketing assets such as trailers, promos, clips, etc.

Framerate Requirements:

*   25 fps media must have subtitles/CC timed to PAL 25 timecode.
*   23.976 (23.98) media must have subtitles/CC timed to either SMPTE 24 timecode or 23.976 Media-Time (timing method must be specified in the file using ttp:timeBase and in the Backlot delivery metadata as either SMPTE or MEDIA). IMSC1.1 documents must only use Media-Time.
*   59.94 fps & 29.97 fps media must have subtitles/CC timed to drop-frame 29.97 timecode using ttp:dropMode. ttp:dropMode is only valid when used in conjunction with ttp:timeBase=”smpte”. As such, ttp:dropMode does not apply to IMSC1.1 documents, which must only be provided using MEDIA timeBase.

To ensure the best quality and consistency please reference our [Timed Text Style Guides](https://partnerhelp.netflixstudios.com/hc/en-us/sections/22463232153235-Timed-Text-Style-Guides-and-Updates).

Acceptable formats:

*   [TTML1](https://www.w3.org/TR/ttml1/) (.xml, .ttml) format (see Netflix [Timed Text Style Guide](https://partnerhelp.netflixstudios.com/hc/en-us/sections/22463232153235-Timed-Text-Style-Guides-and-Updates) for details).
*   [IMSC1.1](http://netflix.com/ns/imsc1.1/text/1) (.xml) - for Japanese subtitles only.

If your text-based subtitle format is not listed above, please contact your Netflix representative to discuss.

* * *

### **3. Forced Narrative Subtitles**

Netflix requires final AV be delivered without burned-in subtitles. In order to support this non-subtitled source, a list of Forced Narratives, if required for the asset, should be delivered by production using the Netflix-provided template found [here](https://docs.google.com/spreadsheets/d/1Dw7IEMCihmC5-gDFjPSif1m5vDPDtCfZgVEJgdUile8/edit#gid%3D1049618852).

Examples of Forced Narrative subtitles include:

*   Any alternate language dialog and on-screen text.
*   Inaudible or hard-to-hear dialog.
*   Dialog or on-screen text that should be called out per creative intent.

Example: If an English-language title contains plot-pertinent Japanese content that an

English-speaking audience should understand, the final AV should not include burned-in subtitles for those instances. The Forced Narrative template should be filled out with the Japanese dialog translated into English, with preferred punctuation and formatting, as well as corresponding in and out-times for the events.

The Forced Narrative list should include:

*   In times and out times for Forced Narrative events.
*   The event as it should appear on screen, including preferred punctuation.

The Forced Narrative list should be uploaded to the Localization bucket in Content Hub as a “Localization Note”.

If delivery of a full Forced Narrative subtitle file is required, the technical format must follow the same rules as standard subtitles as denoted in Section 2.

Framerate Requirements:

*   25 fps media must have subtitles/CC timed to PAL 25 timecode.
*   23.976 (23.98) media must have subtitles/CC timed to either SMPTE 24 timecode or 23.976 Media-Time (timing method must be specified in the file using ttp:timeBase and in the Backlot delivery metadata as either SMPTE or MEDIA). IMSC1.1 documents must only use Media-Time.
*   59.94 fps & 29.97 fps media must have subtitles/CC timed to drop-frame 29.97 timecode using ttp:dropMode. ttp:dropMode is only valid when used in conjunction with ttp:timeBase=”smpte”. As such, ttp:dropMode does not apply to IMSC1.1 documents, which must only be provided using MEDIA timeBase.

For more information, please refer to [Forced Narratives Guidelines and Style Guide for Dubbing](https://partnerhelp.netflixstudios.com/hc/en-us/articles/15063070521363). 

* * *

### **4. Accessibility Files (SDH)**

SDH – Subtitles for the Deaf and Hard of Hearing

**SDH must encompass the spoken dialog intended to be understood in the content. If the content has multiple spoken languages, they all must be translated and present in the SDH file.**

### **4.1** **SDH as Separate File**

When delivering SDH, it must be submitted in one of the acceptable formats listed below:

*   [TTML1](https://www.w3.org/TR/ttml1/) (.xml, .ttml) format (see Netflix [Timed Text Style](https://partnerhelp.netflixstudios.com/hc/en-us/sections/22463232153235-Timed-Text-Style-Guides-and-Updates) Guide for details).
*   [IMSC1.1](http://netflix.com/ns/imsc1.1/text/1)(.xml) - for Japanese subtitles only.

If your SDH format is not listed above, please contact Netflix to discuss other options.

Additionally, they meet the following:

*   Raster image-based SDH will not be accepted.
*   SDH files must conform, within a half second, to the Primary Video Mezzanine that is delivered or to the Netflix-provided Proxy File.
*   SDH files must not be censored or contain advertisements, placards, overlay branding, website link callouts or company credits unless required by law.
*   They must not contain a credit for the SDH creator. They must contain a credit for any translations provided.
*   All SDH files need to start at hour 00. Netflix does not accept the SDH timestamps to start at hour 01.
*   Include positional data in the SDH file if a caption or subtitle would otherwise obscure burned-in text.
*   TTML1 format is required for “Right-to-Left” languages such as Arabic and Hebrew.

Framerate Requirements:

*   25 fps media must have subtitles/CC timed to PAL 25 timecode.
*   23.976 (23.98) media must have subtitles/CC timed to either SMPTE 24 timecode or 23.976 Media-Time (timing method must be specified in the file using ttp:timeBase and in the Backlot delivery metadata as either SMPTE or MEDIA). IMSC1.1 documents must only use Media-Time.
*   59.94 fps & 29.97 fps media must have subtitles/CC timed to drop-frame 29.97 timecode using ttp:dropMode. ttp:dropMode is only valid when used in conjunction with ttp:timeBase=”smpte”. As such, ttp:dropMode does not apply to IMSC1.1 documents, which must only be provided using MEDIA timeBase.

**For more detail, please reference our** [Timed Text Style Guides](https://partnerhelp.netflixstudios.com/hc/en-us/sections/22463232153235-Timed-Text-Style-Guides-and-Updates)**.**

* * *

### **5. Alternate Language and Audio Description Delivery to Backlot**

If alternate language and/or audio description tracks are required under the Agreement, they shall be conformed to the primary digital audio/video asset delivered. Acceptable formats for

alternate-language audio tracks are Atmos BWAV ADM, stereo or multi-channel WAVE Extensible Format (.WAV) as described in section 5.1, or QuickTime format as described in section 5.2. Alternate language and audio description channel configurations must match those of the original language mix.

Please note: Lectern-style dubbing (single narrator speaking the role of each character) is only acceptable for Polish or Vietnamese alternate language audio files, unless otherwise requested by your Netflix Representative. For all other languages and types of content, lip-sync or voice over dubbing (as ordered by your Netflix representative) is required for alternate language audio.

### **5.1** **Acceptable Alternate Language and Audio Description Formats (non-QuickTime)**

<table><tbody><tr><td colspan="2"><strong>WAV Specs</strong></td></tr><tr><td>Audio Codec &amp; Container</td><td>Uncompressed PCM audio in an interleaved WAVE Extensible Format (.wav)</td></tr><tr><td>Sample Rate</td><td>48 kHz</td></tr><tr><td>Bitrate</td><td>Highest bitrate possible (CBR)</td></tr><tr><td>Bit Depth</td><td>24-bit or 16 Bit</td></tr></tbody></table><table><tbody><tr><td colspan="9"><strong>Audio Channel Mapping for WAV (.wav)</strong></td></tr><tr><td><strong>Channel</strong></td><td><strong>1</strong></td><td><strong>2</strong></td><td><strong>3</strong></td><td><strong>4</strong></td><td><strong>5</strong></td><td><strong>6</strong></td><td><strong>7</strong></td><td><strong>8</strong></td></tr><tr><td>5.1+2.0 (Option 1)</td><td>L</td><td>R</td><td>C</td><td>LFE</td><td>Ls</td><td>Rs</td><td>Stereo Left</td><td>Stereo Right</td></tr><tr><td>5.1+2.0 (Option 2)</td><td>L</td><td>C</td><td>R</td><td>Ls</td><td>Rs</td><td>LFE</td><td>Stereo Left</td><td>Stereo Right</td></tr><tr><td>5.1</td><td>L</td><td>R</td><td>C</td><td>LFE</td><td>Ls</td><td>Rs</td><td>&nbsp;</td><td>&nbsp;</td></tr><tr><td>2.0</td><td>Stereo Left</td><td>Stereo Right</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td></tr></tbody></table>

### **5.2** **Acceptable Alternate Language and Audio Description Formats (QuickTime)**

Please note: the labels “Left Total” and “Right Total” are used to label the stereo mix channels only used when 5.1 + 2.0 audio is included in a single file (Options 1-4). If stereo only files are delivered (Options 5 & 6) then the labels “Left” and “Right” are used since there is no ambiguity.

<table><tbody><tr><td colspan="2"><strong>Quicktime Specs</strong></td></tr><tr><td>Audio Codec&nbsp;</td><td>Uncompressed LPCM</td></tr><tr><td>Sample Rate</td><td>48 kHz (Big or Little Endian)</td></tr><tr><td>Bit Depth</td><td>24-bit or 16 Bit</td></tr></tbody></table><table><tbody><tr><td colspan="9"><strong>Audio Channel Mapping for Quicktime (.mov)</strong></td></tr><tr><td><strong>Track</strong></td><td colspan="6"><strong>1</strong></td><td><strong>2</strong></td><td><strong>3</strong></td></tr><tr><td><strong>Channel</strong></td><td><strong>1</strong></td><td><strong>2</strong></td><td><strong>3</strong></td><td><strong>4</strong></td><td><strong>5</strong></td><td><strong>6</strong></td><td><strong>1</strong></td><td><strong>1</strong></td></tr><tr><td>5.1+2.0 (Option 1)</td><td>C</td><td>L</td><td>R</td><td>Ls</td><td>Rs</td><td>LFE</td><td>Stereo Left</td><td>Stereo Right</td></tr></tbody></table><table><tbody><tr><td><strong>Track</strong></td><td><strong>1</strong></td><td><strong>2</strong></td><td><strong>3</strong></td><td><strong>4</strong></td><td><strong>5</strong></td><td><strong>6</strong></td><td><strong>7</strong></td><td><strong>8</strong></td></tr><tr><td><strong>Channel</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>1</strong></td></tr><tr><td>5.1+2.0 (Option 2)</td><td>L</td><td>R</td><td>C</td><td>LFE</td><td>Ls</td><td>Rs</td><td>Stereo Left</td><td>Stereo Right</td></tr></tbody></table><table><tbody><tr><td><strong>Track</strong></td><td colspan="6"><strong>1</strong></td><td colspan="2"><strong>2</strong></td></tr><tr><td><strong>Channel</strong></td><td><strong>1</strong></td><td><strong>2</strong></td><td><strong>3</strong></td><td><strong>4</strong></td><td><strong>5</strong></td><td><strong>6</strong></td><td><strong>1</strong></td><td><strong>2</strong></td></tr><tr><td>5.1+2.0 (Option 3)</td><td>L</td><td>R</td><td>C</td><td>LFE</td><td>Ls</td><td>Rs</td><td>Stereo Left</td><td>Stereo Right</td></tr></tbody></table><table><tbody><tr><td><strong>Track</strong></td><td><strong>1</strong></td><td><strong>2</strong></td><td><strong>3</strong></td><td><strong>4</strong></td><td><strong>5</strong></td><td><strong>6</strong></td><td colspan="2"><strong>7</strong></td></tr><tr><td><strong>Channel</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>2</strong></td></tr><tr><td>5.1+2.0 (Option 4)</td><td>L</td><td>R</td><td>C</td><td>LFE</td><td>Ls</td><td>Rs</td><td>Stereo Left</td><td>Stereo Right</td></tr></tbody></table><table><tbody><tr><td><strong>Track</strong></td><td><strong>1</strong></td><td><strong>2</strong></td><td><strong>3</strong></td><td><strong>4</strong></td><td><strong>5</strong></td><td><strong>6</strong></td><td colspan="2"><strong>7</strong></td></tr><tr><td><strong>Channel</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>1</strong></td><td><strong>2</strong></td></tr><tr><td>5.1+2.0 (Option 4)</td><td>L</td><td>R</td><td>C</td><td>LFE</td><td>Ls</td><td>Rs</td><td>Stereo Left</td><td>Stereo Right</td></tr></tbody></table><table><tbody><tr><td><strong>Track</strong></td><td colspan="8"><strong>1</strong></td></tr><tr><td><strong>Channel</strong></td><td><strong>1</strong></td><td><strong>2</strong></td><td><strong>3</strong></td><td><strong>4</strong></td><td><strong>5</strong></td><td><strong>6</strong></td><td><strong>7</strong></td><td><strong>8</strong></td></tr><tr><td>5.1+2.0 (Option 5)</td><td>L</td><td>R</td><td>C</td><td>LFE</td><td>Ls</td><td>Rs</td><td>Stereo Left</td><td>Stereo Right</td></tr></tbody></table><table><tbody><tr><td><strong>Track</strong></td><td colspan="6"><strong>1</strong></td><td><strong>2</strong></td><td><strong>3</strong></td></tr><tr><td><strong>Channel</strong></td><td><strong>1</strong></td><td><strong>2</strong></td><td><strong>3</strong></td><td><strong>4</strong></td><td><strong>5</strong></td><td><strong>6</strong></td><td><strong>1</strong></td><td><strong>2</strong></td></tr><tr><td>5.1+2.0 (Option 6)</td><td>L</td><td>R</td><td>C</td><td>LFE</td><td>Ls</td><td>Rs</td><td>Stereo Left</td><td>Stereo Right</td></tr></tbody></table><table><tbody><tr><td><strong>Track</strong></td><td colspan="6"><strong>1</strong></td></tr><tr><td><strong>Channel</strong></td><td><strong>1</strong></td><td><strong>2</strong></td><td><strong>3</strong></td><td><strong>4</strong></td><td><strong>5</strong></td><td><strong>6</strong></td></tr><tr><td>5.1</td><td>L</td><td>R</td><td>C</td><td>LFE</td><td>Ls</td><td>Rs</td></tr></tbody></table><table><tbody><tr><td><strong>Track</strong></td><td><strong>1</strong></td><td><strong>2</strong></td></tr><tr><td><strong>Channel</strong></td><td><strong>1</strong></td><td><strong>1</strong></td></tr><tr><td>2.0 (Option 1)</td><td>L</td><td>R</td></tr></tbody></table><table><tbody><tr><td><strong>Track</strong></td><td colspan="2"><strong>1</strong></td></tr><tr><td><strong>Channel</strong></td><td><strong>1</strong></td><td><strong>2</strong></td></tr><tr><td>2.0 (Option 2)</td><td>L</td><td>R</td></tr></tbody></table>

* * *

### **6. Audio Mix Requirements: Alternate Language and Audio Description**

### **6.1** **Audio Prerequisites**

Discrete audio is required, except in the following circumstances:

*   When muxed audio is inherent to the source, such as audio in an IMF, Quicktime or Atmos® BWAV ADM container.
*   Interleaved Secondary Audio .wav deliveries. 

All audio must sync to the final picture, including 1 second of black before the program start FFOA, and 1 second of black after LFOA.

Alternate/Dubbed Language and Audio Description Mixes must not contain an additional leader. 

For all titles, 5.1 audio is required and 2.0 is optional.

Mono audio is acceptable if the program’s original source is mono and no stereo and/or 5.1 mix exists. Mono audio must be duplicated on channels 1 & 2 and delivered as 2-channel.

### **6.2** **Near Field Atmos****®** **Mix - Mastering and Archive - Dubbed Languages and Audio Description**

The Dolby Atmos® Dubbed Language Home Mix must meet the following requirements.

*   At a minimum, must be mixed in a 7.1.4 room.
*   Dolby Certification is not required for Home Atmos® mix rooms.
*   This is a near field mix. The most common monitoring levels for near field are 79db or 82db.
*   Must conform to Netflix loudness spec (-27db LKFS +/- 2 LU 1770-1 dialogue loudness).
*   Peaks should generally not exceed -2dbfs True Peak. To achieve this, we recommend setting True Peak limiters on all beds and objects at -2.3 or lower. Loudness and peaks should be measured via a 5.1 rerender.
*   For native Atmos® mixes, the 5.1 and 2.0 rerenders must conform to Netflix loudness and Peak specification.
*   All beds and objects are encoded and will always be audible. A printmaster may utilize a composite of all bed material OR multiple beds, but not both.
*   For all series/doc/unscripted/comedy content, beds and objects must be separated by Dialog, Music and Effects. For film content, DME separation should be maintained whenever possible.
*   If a 85 db reference theatrical mix is created, two complete sets of deliverables are required. One for theatrical, one for near field.
*   Dubbed Language Atmos® files shall match final IMF picture length exactly as long-play and not separate reels. Leader and sync pop shall be removed.
*   FFOA must be left at default - leave “Add FFOA” box unchecked. For pre-3.0 renderer software, leave red dashes in FFOA value.
*   Final Home Theater Print Master:
    *   Dolby Atmos® BWAV ADM File.
        *   All bed channel configurations are acceptable.
        *   48 kHz, 24 bit.

### **6.3** **Near Field 5.1 Surround Mix - Mastering and Archive - Dubbed Languages and Audio Description**

*   Use 79dB spl or 82dB spl as your standard reference level for mixing.
*   Meet a -27 LKFS (+/- 2 LU) dialog-gated using ITU-R BS.1770-1 measured over entire program.
*   Do not exceed +18db (-2 dBFS) maximum level (true-peak) over reference of -20 dBFS, achieved by peak limiting and not lowering the mix level.
*   For Original Version: Provide 5.1 Dialog, Music and Effects stems that equal the 5.1 mix when combined.
*   For Dubbed Version: Provide 5.1 Dialog stem that equals the 5.1 mix when combined with M&E.

### **6.4** **Near Field 2.0 Stereo Mix - Mastering and Archive - Dubbed Languages and Audio Description**

*   Use 79dB spl or 82dB spl as your standard reference level for mixing.
*   Provide a separate Lo/Ro or LT/RT mix with -27 LKFS (+/- 2 LU) dialogue loudness using ITU-R BS.1770-1 measured over the entire program.
    *   Lo/Ro mix is preferred.
*   Lo/Ro or LT/RT mix to be mono compatible.
*   Do not exceed +18db (-2 dBFS) maximum level (true-peak) over reference of -20 dBFS, achieved by peak limiting and not lowering the mix level.
*   When down-mixing from 5.1 to create Lo/Ro or LT/RT 2.0 mix:
*   Lower Center channel content by -3db.
*   Center channel content should be included in both the LEFT and RIGHT CHANNELS.
*   Lower Surround channel content by a minimum of -3db.
*   Fold Left and Right Surround content into the corresponding LEFT and RIGHT CHANNELS.
*   Optionally include the Low Frequency Effects (LFE) channel between -8db and -12db.
    *   Fold Low Frequency Effects (LFE) into both the LEFT and RIGHT CHANNELS.
    *   Low Pass Filter LFE at 200Hz or lower.
*   All adjustments must be made to the individual 5.1 channels prior to folding down.

**Note:** The resulting 2.0 mix must be checked prior to delivery to ensure it is free of any audio artifacts and if necessary, as determined by Netflix, further adjustments shall be made to prevent them. Any 2.0 delivery must meet the specification prescribed in this section.

* * *

### **7. Dub Cards/Dub Credits**

If dubbed audio files are delivered to backlot and dubs are billed to Netflix and branded, Partner shall enter dub card credits in Netflix’s Dub Talent List tool, which requires Partner to enter talent data - cast and crew - per title. Once talent entry is submitted, the partner has the option to download the dub card deliverables (.zip and .png) for their own archive.

If dubbed audio files are delivered to Netflix and dubs are not billed to Netflix and/or are not branded,

Partner must upload an image based Dub Cards to Netflix formatted exactly as they are to appear on-screen. No extraneous information can be included beyond studio name, cast and other key personnel or as otherwise required by law in the territory of exhibition. Acceptable formats and specifications below.

##### **Acceptable Dub Card Formats**

*   **Image Files**
    *   Each Image must represent one frame of dubbed actor credits.
    *   Only one language can be represented on a dub card and the dubbed language must be specified in the dub card text.
        *   Example: "Version Française"
    *   We accept the following flat file types in order of preference (no layers or pages):
        *   TIFF
        *   PNG
        *   BMP
        *   JPG
    *   Minimum Resolution: 640x480.
    *   Pixel Aspect Ratio (PAR): 1:1 square pixels.

In cases where multiple dub cards are needed for an individual language, the multiple dub cards must be stored in a ZIP archive.

*   ##### **ZIP Archive**
    
    *   Each Image must meet the image file spec described above.
    *   Each image must match the file format and resolution of the other images in the ZIP archive.
    *   All images in ZIP archive must be for the same language.
    *   Images will be rendered to screen in alpha-numeric sorted order (case insensitive).
    *   Acceptable Compression modes: “DEFLATE” or “STORE.”
        *   Note: WinZip and WinRAR use DEFLATE by default.

*   **Note:** the ZIP file name does not need to adhere to any specific convention. Image files contained in the ZIP archive must be named in case-insensitive alphanumeric order.

*   **Examples:**
    *   Brazilian Portuguese
        *   ZIP File name: SomeTitle_pt-BR.zip
        *   Image names: dubCard01.tiff, dubCard02.tiff, dubCard03.tiff
    *   French
        *   ZIP File name: FrenchDubCards.zip
        *   Image names: FrenchActors01.png, FrenchActors02.png, FrenchActors03.png

All dubbed and/or subtitled content is to be accompanied with the relevant metadata in the original and alternate language to support the source delivered.

* * *

### **Appendix**

### **Language Codes**

If the desired language code is not found in the table below please contact your Netflix Representative.

<table><tbody><tr><td><strong>Language Name</strong></td><td><strong>Language Code</strong></td><td><strong>Audio</strong></td><td><strong>Text</strong></td></tr><tr><td>Acoli</td><td>ach</td><td>√</td><td>√</td></tr><tr><td>Afrikaans</td><td>af</td><td>√</td><td>√</td></tr><tr><td>Albanian</td><td>sq</td><td>√</td><td>√</td></tr><tr><td>Amharic</td><td>am</td><td>√</td><td>√</td></tr><tr><td>Arabic</td><td>ar</td><td>√</td><td>√</td></tr><tr><td>Arabic (Algeria)</td><td>ar-DZ</td><td>√</td><td>√</td></tr><tr><td>Arabic (Bahrain)</td><td>ar-BH</td><td>√</td><td>√</td></tr><tr><td>Arabic (Chad)</td><td>ar-TD</td><td>√</td><td>√</td></tr><tr><td>Arabic (Comoros)</td><td>ar-KM</td><td>√</td><td>√</td></tr><tr><td>Arabic (Djibouti)</td><td>ar-DJ</td><td>√</td><td>√</td></tr><tr><td>Arabic (Egypt)</td><td>ar-EG</td><td>√</td><td>√</td></tr><tr><td>Arabic (Eritrea)</td><td>ar-ER</td><td>√</td><td>√</td></tr><tr><td>Arabic (Iraq)</td><td>ar-IQ</td><td>√</td><td>√</td></tr><tr><td>Arabic (Israel)</td><td>ar-IL</td><td>√</td><td>√</td></tr><tr><td>Arabic (Jordan)</td><td>ar-JO</td><td>√</td><td>√</td></tr><tr><td>Arabic (Kuwait)</td><td>ar-KW</td><td>√</td><td>√</td></tr><tr><td>Arabic (Lebanon)</td><td>ar-LB</td><td>√</td><td>√</td></tr><tr><td>Arabic (Libya)</td><td>ar-LY</td><td>√</td><td>√</td></tr><tr><td>Arabic (Mauritania)</td><td>ar-MR</td><td>√</td><td>√</td></tr><tr><td>Arabic (Morocco)</td><td>ar-MA</td><td>√</td><td>√</td></tr><tr><td>Arabic (Oman)</td><td>ar-OM</td><td>√</td><td>√</td></tr><tr><td>Arabic (Palestine)</td><td>ar-PS</td><td>√</td><td>√</td></tr><tr><td>Arabic (Qatar)</td><td>ar-QA</td><td>√</td><td>√</td></tr><tr><td>Arabic (Saudi Arabia)</td><td>ar-SA</td><td>√</td><td>√</td></tr><tr><td>Arabic (Somalia)</td><td>ar-SO</td><td>√</td><td>√</td></tr><tr><td>Arabic (South Sudan)</td><td>ar-SS</td><td>√</td><td>√</td></tr><tr><td>Arabic (Sudan)</td><td>ar-SD</td><td>√</td><td>√</td></tr><tr><td>Arabic (Syria)</td><td>ar-SY</td><td>√</td><td>√</td></tr><tr><td>Arabic (Tunisia)</td><td>ar-TN</td><td>√</td><td>√</td></tr><tr><td>Arabic (United Arab Emirates)</td><td>ar-AE</td><td>√</td><td>√</td></tr><tr><td>Arabic (Western Sahara)</td><td>ar-EH</td><td>√</td><td>√</td></tr><tr><td>Arabic (Yemen)</td><td>ar-YE</td><td>√</td><td>√</td></tr><tr><td>Aramaic</td><td>arc</td><td>√</td><td>√</td></tr><tr><td>Armenian</td><td>hy</td><td>√</td><td>√</td></tr><tr><td>Assamese</td><td>as</td><td>√</td><td>√</td></tr><tr><td>Aymara</td><td>ay</td><td>√</td><td>&nbsp;</td></tr><tr><td>Bambara</td><td>bm</td><td>√</td><td>√</td></tr><tr><td>Bangla</td><td>bn</td><td>√</td><td>√</td></tr><tr><td>Bantu</td><td>bnt</td><td>√</td><td>&nbsp;</td></tr><tr><td>Bashkir</td><td>ba</td><td>√</td><td>√</td></tr><tr><td>Basque</td><td>eu</td><td>√</td><td>√</td></tr><tr><td>Belarusian</td><td>be</td><td>√</td><td>√</td></tr><tr><td>Berber</td><td>ber</td><td>√</td><td>&nbsp;</td></tr><tr><td>Bodo</td><td>brx</td><td>√</td><td>√</td></tr><tr><td>Bosnian</td><td>bs</td><td>√</td><td>√</td></tr><tr><td>Bulbovian</td><td>xa</td><td>√</td><td>√</td></tr><tr><td>Bulgarian</td><td>bg</td><td>√</td><td>√</td></tr><tr><td>Burmese</td><td>my</td><td>√</td><td>√</td></tr><tr><td>Cantonese</td><td>yue</td><td>√</td><td>√</td></tr><tr><td>Catalan</td><td>ca</td><td>√</td><td>√</td></tr><tr><td>Cebuano</td><td>ceb</td><td>√</td><td>&nbsp;</td></tr><tr><td>Chechen</td><td>ce</td><td>√</td><td>√</td></tr><tr><td>Cheyenne</td><td>chy</td><td>√</td><td>√</td></tr><tr><td>Croatian</td><td>hr</td><td>√</td><td>√</td></tr><tr><td>Czech</td><td>cs</td><td>√</td><td>√</td></tr><tr><td>Danish</td><td>da</td><td>√</td><td>√</td></tr><tr><td>Dari</td><td>fa-AF</td><td>√</td><td>√</td></tr><tr><td>Dinka</td><td>din</td><td>√</td><td>√</td></tr><tr><td>Dogri</td><td>doi</td><td>√</td><td>&nbsp;</td></tr><tr><td>Dutch</td><td>nl</td><td>√</td><td>√</td></tr><tr><td>Dzongkha</td><td>dz</td><td>√</td><td>√</td></tr><tr><td>Efik</td><td>efi</td><td>√</td><td>√</td></tr><tr><td>Elamite</td><td>elx</td><td>√</td><td>√</td></tr><tr><td>English</td><td>en</td><td>√</td><td>√</td></tr><tr><td>English (Australia)</td><td>en-AU</td><td>√</td><td>√</td></tr><tr><td>English (Britain)</td><td>en-GB</td><td>√</td><td>√</td></tr><tr><td>English (India)</td><td>en-IN</td><td>√</td><td>√</td></tr><tr><td>English (Kenya)</td><td>en-KE</td><td>√</td><td>√</td></tr><tr><td>English (Nigeria)</td><td>en-NG</td><td>√</td><td>√</td></tr><tr><td>English (Philippines)</td><td>en-PH</td><td>√</td><td>√</td></tr><tr><td>English (South Africa)</td><td>en-ZA</td><td>√</td><td>√</td></tr><tr><td>Esperanto</td><td>eo</td><td>√</td><td>√</td></tr><tr><td>Estonian</td><td>et</td><td>√</td><td>√</td></tr><tr><td>Faroese</td><td>fo</td><td>√</td><td>√</td></tr><tr><td>Filipino</td><td>fil</td><td>√</td><td>√</td></tr><tr><td>Finnish</td><td>fi</td><td>√</td><td>√</td></tr><tr><td>Flemish</td><td>nl-BE</td><td>√</td><td>√</td></tr><tr><td>French</td><td>fr</td><td>√</td><td>√</td></tr><tr><td>French (Canada)</td><td>fr-CA</td><td>√</td><td>√</td></tr><tr><td>Fulah</td><td>ff</td><td>√</td><td>&nbsp;</td></tr><tr><td>Galician</td><td>gl</td><td>√</td><td>√</td></tr><tr><td>Georgian</td><td>ka</td><td>√</td><td>√</td></tr><tr><td>German</td><td>de</td><td>√</td><td>√</td></tr><tr><td>Gogo</td><td>gog</td><td>√</td><td>√</td></tr><tr><td>Greek</td><td>el</td><td>√</td><td>√</td></tr><tr><td>Gujarati</td><td>gu</td><td>√</td><td>√</td></tr><tr><td>Hausa</td><td>ha</td><td>√</td><td>√</td></tr><tr><td>Hawaiian</td><td>haw</td><td>√</td><td>√</td></tr><tr><td>Hebrew</td><td>he</td><td>√</td><td>√</td></tr><tr><td>Hindi</td><td>hi</td><td>√</td><td>√</td></tr><tr><td>Hindi (Latin)</td><td>hi-Latn</td><td>&nbsp;</td><td>√</td></tr><tr><td>Hokkien</td><td>nan</td><td>√</td><td>√</td></tr><tr><td>Hungarian</td><td>hu</td><td>√</td><td>√</td></tr><tr><td>Icelandic</td><td>is</td><td>√</td><td>√</td></tr><tr><td>Igbo</td><td>ig</td><td>√</td><td>√</td></tr><tr><td>Ijaw</td><td>ijo</td><td>√</td><td>√</td></tr><tr><td>Indonesian</td><td>id</td><td>√</td><td>√</td></tr><tr><td>Inuktitut</td><td>iu</td><td>√</td><td>√</td></tr><tr><td>Irish</td><td>ga</td><td>√</td><td>√</td></tr><tr><td>Italian</td><td>it</td><td>√</td><td>√</td></tr><tr><td>Jamaican Patois</td><td>jam</td><td>√</td><td>√</td></tr><tr><td>Japanese</td><td>ja</td><td>√</td><td>√</td></tr><tr><td>Javanese</td><td>jv</td><td>√</td><td>√</td></tr><tr><td>Kannada</td><td>kn</td><td>√</td><td>√</td></tr><tr><td>Kashmiri</td><td>ks</td><td>√</td><td>√</td></tr><tr><td>Kazakh</td><td>kk</td><td>√</td><td>√</td></tr><tr><td>Khasi</td><td>kha</td><td>√</td><td>√</td></tr><tr><td>Khmer</td><td>km</td><td>√</td><td>√</td></tr><tr><td>Kikuyu</td><td>ki</td><td>√</td><td>√</td></tr><tr><td>Kinyarwanda</td><td>rw</td><td>√</td><td>√</td></tr><tr><td>Klingon</td><td>tlh</td><td>√</td><td>√</td></tr><tr><td>Konkani</td><td>kok</td><td>√</td><td>√</td></tr><tr><td>Korean</td><td>ko</td><td>√</td><td>√</td></tr><tr><td>Kurdish</td><td>ku</td><td>√</td><td>√</td></tr><tr><td>Kyrgyz</td><td>ky</td><td>√</td><td>√</td></tr><tr><td>Lango (Uganda)</td><td>laj</td><td>√</td><td>√</td></tr><tr><td>Lao</td><td>lo</td><td>√</td><td>√</td></tr><tr><td>Latin</td><td>la</td><td>√</td><td>√</td></tr><tr><td>Latvian</td><td>lv</td><td>√</td><td>√</td></tr><tr><td>Lingala</td><td>ln</td><td>√</td><td>√</td></tr><tr><td>Lithuanian</td><td>lt</td><td>√</td><td>√</td></tr><tr><td>Luxembourgish</td><td>lb</td><td>√</td><td>√</td></tr><tr><td>Macedonian</td><td>mk</td><td>√</td><td>√</td></tr><tr><td>Maithili</td><td>mai</td><td>√</td><td>&nbsp;</td></tr><tr><td>Malagasy</td><td>mg</td><td>√</td><td>√</td></tr><tr><td>Malay</td><td>ms</td><td>√</td><td>√</td></tr><tr><td>Malayalam</td><td>ml</td><td>√</td><td>√</td></tr><tr><td>Maltese</td><td>mt</td><td>√</td><td>√</td></tr><tr><td>Mandarin</td><td>zh</td><td>√</td><td>&nbsp;</td></tr><tr><td>Mandarin (Mainland China)</td><td>zh-CN</td><td>√</td><td>&nbsp;</td></tr><tr><td>Mandarin (Taiwan)</td><td>zh-TW</td><td>√</td><td>&nbsp;</td></tr><tr><td>Mandingo</td><td>man</td><td>√</td><td>&nbsp;</td></tr><tr><td>Manipuri</td><td>mni</td><td>√</td><td>√</td></tr><tr><td>Maori</td><td>mi</td><td>√</td><td>√</td></tr><tr><td>Marathi</td><td>mr</td><td>√</td><td>√</td></tr><tr><td>Masai</td><td>mas</td><td>√</td><td>√</td></tr><tr><td>Mayan</td><td>myn</td><td>√</td><td>√</td></tr><tr><td>Mende</td><td>men</td><td>√</td><td>√</td></tr><tr><td>Mongolian</td><td>mn</td><td>√</td><td>√</td></tr><tr><td>Multiple languages</td><td>mul</td><td>√</td><td>√</td></tr><tr><td>Nepali</td><td>ne</td><td>√</td><td>√</td></tr><tr><td>Newari</td><td>new</td><td>√</td><td>√</td></tr><tr><td>Nigerian Pidgin</td><td>pcm</td><td>√</td><td>√</td></tr><tr><td>No linguistic content</td><td>zxx</td><td>√</td><td>√</td></tr><tr><td>North Ndebele</td><td>nd</td><td>√</td><td>√</td></tr><tr><td>Northern Sami</td><td>se</td><td>√</td><td>√</td></tr><tr><td>Northern Sotho</td><td>nso</td><td>√</td><td>√</td></tr><tr><td>Norwegian</td><td>nb</td><td>√</td><td>√</td></tr><tr><td>Nyanja</td><td>ny</td><td>√</td><td>&nbsp;</td></tr><tr><td>Odia</td><td>or</td><td>√</td><td>√</td></tr><tr><td>Oromo</td><td>om</td><td>√</td><td>&nbsp;</td></tr><tr><td>Papiamento</td><td>pap</td><td>&nbsp;</td><td>√</td></tr><tr><td>Pashto</td><td>ps</td><td>√</td><td>√</td></tr><tr><td>Persian</td><td>fa</td><td>√</td><td>√</td></tr><tr><td>Polish</td><td>pl</td><td>√</td><td>√</td></tr><tr><td>Portuguese (Brazil)</td><td>pt-BR</td><td>√</td><td>√</td></tr><tr><td>Portuguese (Portugal)</td><td>pt</td><td>√</td><td>√</td></tr><tr><td>Punjabi</td><td>pa</td><td>√</td><td>√</td></tr><tr><td>Quechua</td><td>qu</td><td>√</td><td>√</td></tr><tr><td>Quechua (Bolivia)</td><td>qu-BO</td><td>√</td><td>√</td></tr><tr><td>Quechua (Ecuador)</td><td>qu-EC</td><td>√</td><td>√</td></tr><tr><td>Quechua (Peru)</td><td>qu-PE</td><td>√</td><td>√</td></tr><tr><td>Romanian</td><td>ro</td><td>√</td><td>√</td></tr><tr><td>Romansh</td><td>rm</td><td>√</td><td>√</td></tr><tr><td>Romany</td><td>rom</td><td>√</td><td>√</td></tr><tr><td>Russian</td><td>ru</td><td>√</td><td>√</td></tr><tr><td>Sami</td><td>smi</td><td>√</td><td>√</td></tr><tr><td>Samoan</td><td>sm</td><td>√</td><td>√</td></tr><tr><td>Sanskrit</td><td>sa</td><td>√</td><td>√</td></tr><tr><td>Santali</td><td>sat</td><td>√</td><td>&nbsp;</td></tr><tr><td>Scottish Gaelic</td><td>gd</td><td>√</td><td>√</td></tr><tr><td>Serbian</td><td>sr</td><td>√</td><td>&nbsp;</td></tr><tr><td>Serbian (Cyrillic)</td><td>sr-Cyrl</td><td>&nbsp;</td><td>√</td></tr><tr><td>Serbian (Latin)</td><td>sr-Latn</td><td>&nbsp;</td><td>√</td></tr><tr><td>Sherdukpen</td><td>sdp</td><td>√</td><td>√</td></tr><tr><td>Shona</td><td>sn</td><td>√</td><td>&nbsp;</td></tr><tr><td>Simplified Chinese</td><td>zh-Hans</td><td>&nbsp;</td><td>√</td></tr><tr><td>Sindhi</td><td>sd</td><td>√</td><td>&nbsp;</td></tr><tr><td>Sinhala</td><td>si</td><td>√</td><td>√</td></tr><tr><td>Slovak</td><td>sk</td><td>√</td><td>√</td></tr><tr><td>Slovenian</td><td>sl</td><td>√</td><td>√</td></tr><tr><td>Somali</td><td>so</td><td>√</td><td>√</td></tr><tr><td>Songhai</td><td>son</td><td>√</td><td>√</td></tr><tr><td>South Ndebele</td><td>nr</td><td>√</td><td>√</td></tr><tr><td>Southern Sotho</td><td>st</td><td>√</td><td>√</td></tr><tr><td>Spanish (Latam)</td><td>es</td><td>√</td><td>√</td></tr><tr><td>Spanish (Argentina)</td><td>es-AR</td><td>√</td><td>√</td></tr><tr><td>Spanish (Colombia)</td><td>es-CO</td><td>√</td><td>√</td></tr><tr><td>Spanish (Mexico)</td><td>es-MX</td><td>√</td><td>√</td></tr><tr><td>Spanish (Spain)</td><td>es-ES</td><td>√</td><td>√</td></tr><tr><td>Swahili</td><td>sw</td><td>√</td><td>√</td></tr><tr><td>Swati</td><td>ss</td><td>√</td><td>√</td></tr><tr><td>Swedish</td><td>sv</td><td>√</td><td>√</td></tr><tr><td>Swiss German</td><td>gsw</td><td>√</td><td>√</td></tr><tr><td>Taiwanese</td><td>nan-TW</td><td>√</td><td>&nbsp;</td></tr><tr><td>Tamashek</td><td>tmh</td><td>√</td><td>√</td></tr><tr><td>Tamil</td><td>ta</td><td>√</td><td>√</td></tr><tr><td>Taroko</td><td>trv</td><td>√</td><td>&nbsp;</td></tr><tr><td>Telugu</td><td>te</td><td>√</td><td>√</td></tr><tr><td>Thai</td><td>th</td><td>√</td><td>√</td></tr><tr><td>Tibetan</td><td>bo</td><td>√</td><td>√</td></tr><tr><td>Tongan</td><td>to</td><td>√</td><td>√</td></tr><tr><td>Traditional Chinese</td><td>zh-Hant</td><td>&nbsp;</td><td>√</td></tr><tr><td>Traditional Chinese (Hong Kong)</td><td>zh-Hant-HK</td><td>&nbsp;</td><td>√</td></tr><tr><td>Tsonga</td><td>ts</td><td>√</td><td>√</td></tr><tr><td>Tswana</td><td>tn</td><td>√</td><td>√</td></tr><tr><td>Turkish</td><td>tr</td><td>√</td><td>√</td></tr><tr><td>Tuvinian</td><td>tyv</td><td>√</td><td>√</td></tr><tr><td>Ugaritic</td><td>uga</td><td>√</td><td>√</td></tr><tr><td>Ukrainian</td><td>uk</td><td>√</td><td>√</td></tr><tr><td>Urdu</td><td>ur</td><td>√</td><td>√</td></tr><tr><td>Venda</td><td>ve</td><td>√</td><td>√</td></tr><tr><td>Vietnamese</td><td>vi</td><td>√</td><td>√</td></tr><tr><td>Welsh</td><td>cy</td><td>√</td><td>√</td></tr><tr><td>Wolof</td><td>wo</td><td>√</td><td>√</td></tr><tr><td>Xhosa</td><td>xh</td><td>√</td><td>√</td></tr><tr><td>Yiddish</td><td>yi</td><td>√</td><td>√</td></tr><tr><td>Yoruba</td><td>yo</td><td>√</td><td>√</td></tr><tr><td>Zapotec</td><td>zap</td><td>√</td><td>√</td></tr><tr><td>Zulu</td><td>zu</td><td>√</td><td>√</td></tr></tbody></table>

* * *

### **Translations**

*   [العربية‬](https://drive.google.com/file/d/149fRRSOd3dWWUXAhzjy1pIgNLzS4TgDi/view?usp=drive_link)
*   [Español (España)](https://drive.google.com/file/d/1ddislMWD4SOiCqS2577919MsMoUwKUvx/view?usp=drive_link)
*   [Español (Latinoamérica)](https://drive.google.com/file/d/1kgej_JeteFRFxYM5mm1ogOffNOGwlXBq/view?usp=drive_link)
*   [Français](https://drive.google.com/file/d/1Jl-A_T55ZOETO_L05CDHZToiDhQdxY8F/view?usp=drive_link)
*   [Indonesian](https://drive.google.com/file/d/1_H2Kb6f89bU3f8bI_pWGfE5tRLyrxoq_/view?usp=drive_link)
*   [Italiano](https://drive.google.com/file/d/1LEnP3fiBdgZ-4tQCTiNxCHtLRG7RPpdc/view?usp=drive_link)‬
*   [日本語](https://drive.google.com/file/d/1z6coIxINLwwFMt3U9QAPvyHBZCQY87CJ/view?usp=drive_link)
*   [한국어](https://drive.google.com/file/d/1rfV7QYA45dyUIfNZMwyyINNVm0LhrsOm/view?usp=drive_link)
*   [Polski](https://drive.google.com/file/d/1VfGCO00H4yYFRQGVUkPXu6uwiCa40mDP/view?usp=drive_link)  
    
*   [Português](https://drive.google.com/file/d/1D5RW2sdGDOT0VsGYk18oiXeujoKJQM0V/view?usp=drive_link)
*   [Türkçe](https://drive.google.com/file/d/1-vgGZvUybiMvkWyPfoqwxCsNt2ukgLMt/view?usp=drive_link)
*   [繁體中文](https://drive.google.com/file/d/1si9LjjEI-4i45yXoMiaknWujuijzoIXY/view?usp=drive_link)  
    

* * *

### **Change Log**

**09/12/2023**

*   Section 1: updated language to align with English timed text style guide.
*   Section 1: Removed language regarding PSE (Photosensitive Epilepsy) requirements for animated content and added it to the Post Production Branded Delivery Specifications v5.1.
*   Section 3: Added additional reference link to supporting documentation: [Forced Narratives Guidelines and Style Guide for Dubbing](https://partnerhelp.netflixstudios.com/hc/en-us/articles/15063070521363-Forced-Narratives-Guidelines-and-Style-) .
*   Sections 5.1 & 5.2: Converted specs to table format for readability. 
*   Section 5.2: Corrected Option 5 of 5.1+2.0 channel mapping for quicktime to be 1 Track instead of 8.
*   Section 5.2: Added a 6th Option for acceptable 5.1+2.0 audio channel mapping for quicktime.
*   Section 5.2: Added 5.1 only option.
*   Section 6: Streamlined and clarified language throughout.
*   Appendix: Added updated localization codes for English (Kenya), English (Nigeria), English (Philippines), Spanish (Colombia), Galician, Gogo, Ijaw, Lao, Nigerian Pidgin, Northern Sami.

**06/24/2022**

*   **Netflix Branded Delivery Specifications OC-4-1 has been split into three new specification resources.**
    *   Post Production Branded Delivery Specifications v1.0
    *   Marketing & Promotional Branded Delivery Specifications v1.0
    *   Localization, Accessibility, & Dubbing Delivery Specifications v1.0
*   What was previously section 5, “Secondary Asset Specifications,” has been moved to Localization, Accessibility, and Dubbing Delivery Specifications v1.0.
*   What was previously section 6 “Movie Content Metadata” has been removed.
*   What was previously section 8, “Textless Version IMF Package” has been moved into section 2, “IMF specifications.”
*   The dubbing elements previously from Section 4.2 “Audio Mix Requirements,” have been moved to Localization, Accessibility, and Dubbing Delivery Specifications v 1.0
*   What was previously section 7, “Delivery Platforms” has been removed.
*   What was previously section 11, “Promotional Assets and Source Materials” has been moved to Marketing & Promotional Branded Delivery Specifications v1.0
*   What was previously section 12.1 “Language Codes” has been moved to Localization, Accessibility and Dubbing Delivery Specifications  v 1.0

Was this article helpful? 0 out of 1 found this helpful