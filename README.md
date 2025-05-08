- This is a work sample of an audio preservation and restoration project I've done. Audio samples are available in the folder. Due to GitHub's file size limitations, only compressed (MP3) versions are included.
- Audio files without the RX_ prefix are the original digitized versions. Files with the RX_ prefix are the restored versions.
- The following texts document all the Metadata and processing steps regarding the vinyl recording digitization and restoration. 




---
### <div align="center">**Record Preservation and Restoration Metadata** </div>

<div align="center"><img width="299" alt="Image" src="https://github.com/user-attachments/assets/98a28049-c8f1-426c-b132-fab4d9cf6bbe" />
<img width="295" alt="Image" src="https://github.com/user-attachments/assets/c7ea5caf-b4bd-4c91-8604-222a83028944" /> </div>


Title | [The Varsity Seven](https://www.discogs.com/artist/1524495-Varsity-Seven) – Scratch My Back / Save It Pretty Mama
-- | --
Label | Varsity
Company | Varsity
Recording Date | 12/14/1939
Recording Location | New York
Matrix / Runout (Side A label) | US1160
Matrix / Runout (Side B label) | US1161
Genre | Jazz
Format | Shellac, 10", 78 RPM
Artist | Varsity Seven, band members are Danny Polo (clarinet), Benny Carter (alto saxophone, trumpet), Coleman Hawkins (tenor saxophone), Joe Sullivan (piano), Ulysses Livingston (guitar), Artie Shapiro (bass), George Wettling (drums) and Joe Turner (vocals -1,2).
Related Information | The song Save it pretty, mama's original version is performed by Louis Armstrong & His Savoy Ballroom Five in 1929 from Odeon record label, after that there are seven versions performed by different artists and issued by different record labels.
Physical Grade | Good to Fair. The vinyl record has continuous low-level crackles and pops throughout, though they are not loud enough to render the music unlistenable or unenjoyable for the casual listener. The LP cover shows various signs of wear and tear and has been partially repaired with tape.

---
### Digitalizing Process

#### Initial Test
- Installation of a 3-micron diameter stylus was conducted, followed by placement of the disc on the turntable.
- Upon activation, the speed indicator and strobe illuminator were illuminated.
- The rotation speed was adjusted to 78 RPM to align with the record specifications, and the Start/Stop button was engaged to initiate turntable platter rotation.
- The tone arm was positioned over the outer groove, with the cueing lever set to the down position, facilitating a gradual descent of the tone arm onto the record.
- Instability in the needle was observed due to disc rotation, resulting in a rapid traverse from the outer to the inner groove.
- Inspection of the stylus revealed it to be broken.
- Utilization of the phonograph's native stylus yielded a clear sound, albeit with some noise.

#### Recording Test
- Connection of the phonograph to an A/D converter was established through the Audio Archival Preamp MKII, ensuring reproduction of the phonograph disc sound without coloration or added background noise.
- Equalization was set to 78.
- Recording was initiated via Pro Tools, with the volume initially set to the minimum and subsequently increased gradually to achieve a balance between volume and wave.

#### Recording
- The presence of sharp noise was noted, although the music remained clear due to the distinct separation of noise and music frequencies.
- During the recording of Side B, distinct distortions were detected, indicative of the stylus jumping and trembling within the groove.
- The phonograph's native stylus was determined to be thicker than the correct stylus, which features a truncated tip.


---
### Metadata Archival Digital File
Recording Data |  
-- | --
Playback machine | Rek-O-kut Direct Drive Restoration Deck
Analog to digital converter | Audiophile Archival Preamp MKII
Recording software | Pro Tools
Digitalizing time | 11-19-2014, 4:51 pm
Digitalizing location | 35 West 4th Street, New York, NY 10012, USA

### Audio File Metadata (Uncompressed)

| File Content          | Scratch my back | Save it pretty, mama |
|----------------------|-----------------|----------------------|
|  **Name** | Scratchmyback_VarsitySeven | Saveitprettymama_VarsitySeven
| **Sampling Rate**    | 96 kHz          | 96 kHz               |
| **Bit Depth**        | 24 Bit          | 24 Bit               |
| **File Format**      | .wav            | .wav                 |
| **Duration**        | 3'23"           | 3'14"                |
| **File Size**       | 117.3 MB        | 112.1 MB             |

### Audio File Metadata (Compressed)

| File Content          | Scratch my back | Save it pretty, mama |
|----------------------|-----------------|----------------------|
|  **Name** | Scratchmyback_VarsitySeven | Saveitprettymama_VarsitySeven
| **Sampling Rate**    | 44.1 kHz        | 44.1 kHz             |
| **Bit Depth**        | -               | -                    |
| **File Format**      | 128 kbps MP3    | 128 kbps MP3         |
| **Duration**        | 3'23"           | 3'14"                |
| **File Size**       | 8.1 MB          | 7.8 MB               |

---
### Audio Restoration Steps (iZotope RX 3)

#### 1. Broad Noise Reduction
Tool: Spectral De-noise (Modern algorithm)
Steps:
- Capture noise profile from silent groove section (1-2 sec)
- Apply gentle reduction:
   - Threshold: -24 dB 
   - Reduction: 6-12 dB 
- Process in 2-3 passes
 
#### 2. Click/Pop Removal
Tool: Declick (Multiband mode)
Parameters:
- Sensitivity: 4.0 
- Frequency Skew: 8.6 (mid/high focus)
- Click Widening: 2.5 ms

#### 3. Residual Noise Cleanup
Tool: Spectral Repair
Method:
- Zoom to 256-512 FFT resolution
- Use "Attenuate" mode (preserves harmonics)
- Target only visible noise spikes
   
### Restored Audio File Metadata (Uncompressed)
 | File Content | Scratch my back | Save it pretty, mama |
 |-------------|---------------------|----------------|
 |  **Name** | RX_Scratchmyback_VarsitySeven | RX_Saveitprettymama_VarsitySeven
 | **Sampling Rate** | 44.1 kHz | 44.1 kHz |
 | **Bit Depth** | 16 Bit | 16 Bit |
 | **File Format** | .wav | .wav |
 | **Duration** | 3'18" | 3'04" |
 | **File Size** | 76.1 MB | 70.5 MB |

### Restored  Audio File Metadata (compressed)
| File Content | Scratch my back | Save it pretty, mama |
|-------------|---------------------|----------------|
|  **Name** | RX_Scratchmyback_VarsitySeven | RX_Saveitprettymama_VarsitySeven
|  **Sampling Rate** | 44.1 kHz | 44.1 kHz | 
| **Bit Depth**        | -               | -                    |
|  **File Format** | 128 kbps MP3 | 128 kbps MP3 |
|  **Duration** |3'18" | 3'04" | 
|  **File Size** | 7.9 MB | 7.3 MB| 
