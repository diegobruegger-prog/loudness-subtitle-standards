# Loudness and subtitle standards 2026

LUFS and true peak targets for Spotify, Apple Music, YouTube, Netflix, Prime Video, EBU R128, ATSC A/85, podcasts and social video, subtitle rules (Netflix, BBC, YouTube) and frame rates with drop frame. Every value is sourced.

**Browse it with filters and sources:** https://shortformkit.com/loudness-subtitle-standards-2026/

Updated 2026-10-13. Files in [`data/`](data/): one JSON with everything and one CSV per table.

## Loudness targets (23 rows)

Sources for every row are in the CSV/JSON (`sources` column).

| name | category | integrated lufs | tolerance | true peak max dbtp | confidence |
|---|---|---|---|---|---|
| Spotify | music streaming | -14 |  | -1 | high |
| Apple Music (Sound Check) | music streaming | -16 |  |  | medium |
| YouTube (incl. Shorts) | video platform | -14 |  |  | medium |
| Amazon Music | music streaming | -14 |  |  | low |
| TIDAL | music streaming | -14 |  |  | medium |
| Deezer | music streaming | -15 |  |  | medium |
| SoundCloud | music streaming | -14 |  | -1 | high |
| Netflix (branded content, near-field mixes) | streaming video | -27 | ±2 LU | -2 | high |
| Amazon Prime Video / Amazon MGM Studios productions | streaming video | -27 | ±2 LU | -2 | high |
| Disney+ | streaming video | -27 |  | -2 | low |
| EBU R 128 (European broadcast) | broadcast | -23 | ±1.0 LU only where the target is not practically achievable (e.g. live); ±0.2 LU allowed for measurement error in QC | -1 | high |
| EBU R 128 s1 (short-form: ads, promos) | broadcast | -23 | ±0.2 LU (QC measurement tolerance) | -1 | high |
| EBU R 128 s2 (broadcasters' streaming) | streaming video | -23 | interim Distribution Loudness -20.0 to -16.0 LUFS allowed if no loudness metadata is used |  | high |
| ATSC A/85 (US broadcast, CALM Act) | broadcast | -24 | ±2 dB (measurement variation; content should not be targeted to either side) | -2 | high |
| ARIB TR-B32 (Japan broadcast) | broadcast | -24 | ±2 LU (industry preset; not verified in the official text) | -1 | medium |
| AES TD1004.1.15-10 (2015, superseded) | music streaming | -16 to -20 |  | -1 | medium |
| AES TD1008 / AES77-2023 (speech, podcasts) | podcast/audiobook | -18 | +2 LU upper tolerance for speech (industry summary) |  | medium |
| AES TD1008 / AES77-2023 (music) | music streaming | -16 |  |  | medium |
| Apple Podcasts | podcast/audiobook | -16 | ±1 dB | -1 | high |
| Audible / ACX (audiobooks) | podcast/audiobook |  | RMS between -23 dB and -18 dB |  | high |
| Instagram Reels | social | -14 | ±1 LU (observed, not a published spec) |  | medium |
| TikTok | social |  |  |  | medium |
| Facebook (video, Reels) | social |  |  |  | low |

## Subtitle standards (39 rows)

Sources for every row are in the CSV/JSON (`sources` column).

| name | rule | value | applies to |
|---|---|---|---|
| Netflix Timed Text Style Guide | Maximum lines per subtitle | 2 | All languages (Netflix originals and non-originals) |
| Netflix Timed Text Style Guide | Minimum event duration | 5/6 second (20 frames at 24 fps) | All languages except where a language guide overrides (see Japanese) |
| Netflix Timed Text Style Guide | Maximum event duration | 7 seconds | All languages |
| Netflix Timed Text Style Guide | Minimum gap between subtitles (frame gap) | 2 frames | All frame rates |
| Netflix Timed Text Style Guide | Out-time after end of speech | about 0.5 s after audio ends when no subtitle follows | All languages |
| Netflix Timed Text Style Guide | Positioning | Center-justified, top or bottom of screen | All languages; Japanese may use vertical positioning |
| Netflix Timed Text Style Guide | Characters per line | 42 | English (USA) |
| Netflix Timed Text Style Guide | Reading speed | Adult: up to 20 cps; Children: up to 17 cps | English (USA), subtitles and SDH |
| Netflix Timed Text Style Guide | Characters per line | 42 | German |
| Netflix Timed Text Style Guide | Reading speed | Subtitles: adult up to 17 cps, children up to 13 cps; SDH may increase to adult 20 cps, children 17 cps | German |
| Netflix Timed Text Style Guide | Characters per line | 42 | French (France) |
| Netflix Timed Text Style Guide | Reading speed | Subtitles: adult up to 17 cps, children up to 13 cps; SDH may increase to adult 20 cps, children 17 cps | French (France) |
| Netflix Timed Text Style Guide | Characters per line | 42 | Spanish (Latin America & Spain) |
| Netflix Timed Text Style Guide | Reading speed | Adult: up to 17 cps; Children: up to 13 cps (subtitles and SDH) | Spanish (Latin America & Spain) |
| Netflix Timed Text Style Guide | Characters per line | 42 | Italian |
| Netflix Timed Text Style Guide | Reading speed | Adult: up to 17 cps; Children: up to 13 cps | Italian subtitles |
| Netflix Timed Text Style Guide | Characters per line | 42 | Portuguese (Brazil) |
| Netflix Timed Text Style Guide | Reading speed | Subtitles: adult up to 17 cps, children up to 13 cps; SDH: adult up to 20 cps, children up to 17 cps | Portuguese (Brazil) |
| Netflix Timed Text Style Guide | Characters per line | Horizontal: max 13 full-width characters; vertical: max 11 full-width characters (half-width character/space/punctuation counts as 0.5) | Japanese |
| Netflix Timed Text Style Guide | Reading speed | Up to 4 characters per second | Japanese |
| Netflix Timed Text Style Guide | Minimum event duration | 0.5 s (12 frames at 24 fps) | Japanese (overrides the general 5/6 s) |
| Netflix Timed Text Style Guide | Characters per line | 16 (Latin characters, spaces, punctuation count as 0.5) | Korean |
| Netflix Timed Text Style Guide | Reading speed | Subtitles: adult up to 12 cps, children up to 9 cps; SDH adult up to 14 cps | Korean |
| Netflix Timed Text Style Guide | TTML technical rules | Percentage values only (no pixels); tts:fontSize = 100%; positioning via tts:textAlign/tts:displayAlign with static tts:extent/tts:origin | All TTML subtitle and SDH files for Netflix |
| BBC Subtitle Guidelines | Line length (broadcast) | 37 fixed-width characters (Teletext), fewer if coloured text is used | BBC broadcast subtitles |
| BBC Subtitle Guidelines | Line length (online) | 68% of video width for 16:9; 90% for 4:3, 1:1 and 9:16 | BBC online subtitles |
| BBC Subtitle Guidelines | Maximum lines | 2 for 16:9, 4:3 and 1:1; 3 for vertical 9:16 | BBC subtitles |
| BBC Subtitle Guidelines | Subtitle speed | 160-180 words per minute (0.33 to 0.375 s per word); aim for at least about 0.3 s per word on screen | BBC pre-recorded subtitles; live subtitle word rate also 160-180 wpm |
| BBC Subtitle Guidelines | Gaps between subtitles | If a gap is left: minimum 1 second, preferably 1.5 seconds | BBC subtitles |
| BBC Subtitle Guidelines | Delivery formats | EBU-TT-D (online only) or EBU-TT 1.0 (broadcast and online); STL file rules documented separately | BBC deliveries |
| YouTube | Supported basic caption formats | SubRip .srt; SubViewer .sbv/.sub; MPsub .mpsub; LRC .lrc; Videotron Lambda .cap | YouTube uploads |
| YouTube | Supported advanced caption formats | SAMI .smi/.sami; RealText .rt; WebVTT .vtt; TTML .ttml (incl. iTT); DFXP .dfxp/.ttml | YouTube uploads |
| YouTube | Supported broadcast caption formats | Scenarist .scc (preferred, CEA-608); EBU-STL .stl; Caption Center .tds; Cheetah .cap; NCI .cap | YouTube uploads |
| EBU subtitle formats | EBU STL (Tech 3264) | Binary file format for exchange of teletext and in-vision subtitles between broadcasters | Broadcast exchange (legacy, still accepted by YouTube and BBC workflows) |
| EBU subtitle formats | EBU-TT Part 1 (Tech 3350) | XML (TTML-based) archiving and interchange format; current v1.2, May 2017 (v1.0 July 2012) | Archiving and broadcaster interchange |
| EBU subtitle formats | EBU-TT-D (Tech 3380) | XML (TTML-based) format for distribution over IP; current v1.0.1, May 2018, aligned with W3C IMSC 1.0.1 | Online/OTT distribution |
| SRT (SubRip) | File structure | Numeric counter; timing line HH:MM:SS,mmm --> HH:MM:SS,mmm (comma before milliseconds, arrow is two hyphens + '>'); one or more text lines; blank line ends the cue | Any SRT file |
| WebVTT (W3C) | File structure | UTF-8 text, MIME type text/vtt; optional BOM then the string 'WEBVTT' on the first line, followed by a blank line; cue = optional identifier, timing line, payload | Any WebVTT file |
| WebVTT (W3C) | Timestamp format | [hh:]mm:ss.ttt with a full stop before exactly 3 millisecond digits; hours optional unless non-zero; start --> end with spaces | Any WebVTT file |

## Frame rates timecode (9 rows)

Sources for every row are in the CSV/JSON (`sources` column).

| name | exact rate | used for | timecode |
|---|---|---|---|
| 23.976 fps (often shown as 23.98) | 24000/1001 (24 ÷ 1.001) | North American HDTV and 'NTSC film' (24p material in 60 Hz-derived systems) | Non-drop frame only; no drop-frame variant exists |
| 24 fps | 24/1 | Film/cinema, ATSC, 2K/4K digital production | Non-drop frame |
| 25 fps | 25/1 | PAL and SECAM regions (Europe, Australia, parts of South America), DVB; also allowed in ATSC | Non-drop frame; 50i broadcast carries 25 interlaced frames per second |
| 29.97 fps non-drop (NDF) | 30000/1001 (30 ÷ 1.001) | NTSC regions (US, Canada, Mexico, Colombia et al.), ATSC, PAL-M (Brazil) | Counts 30 frame numbers per second continuously, so one hour of 29.97 NDF timecode runs 3.6 s longer than wall-clock time; 00:59:56:12 NDF equals 01:00:00;00 DF |
| 29.97 fps drop frame (DF) | 30000/1001 | Broadcast deliveries in NTSC regions where timecode must match clock time | Skips frame NUMBERS 00 and 01 at the start of every minute except minutes divisible by 10 (00, 10, 20, 30, 40, 50): 18 numbers per 10 minutes, 108 per hour, so one hour holds 107,892 frames instead of 108,000. No picture… |
| 30 fps | 30/1 | ATSC; common web/phone capture rate (YouTube lists 30 as common) | Non-drop frame |
| 50 fps | 50/1 | 50 Hz (PAL-derived) HD progressive systems (BT.709 50/P); high-frame-rate web uploads (YouTube lists 50 as common) | Non-drop frame |
| 59.94 fps | 60000/1001 (60 ÷ 1.001) | 60 Hz-derived (NTSC-region) HD progressive (BT.709 60/1.001); also the field rate of 1080i/480i NTSC broadcast | Drop-frame variant exists: skips 4 frame numbers at each affected minute boundary (same every-minute-except-tenth rule as 29.97 DF) |
| 60 fps | 60/1 | 60 Hz HD progressive (BT.709 60/P); high-frame-rate web uploads (YouTube lists 60 as common) | Non-drop frame |

## How to cite

Shortform Kit (2026), Loudness and subtitle standards 2026, https://shortformkit.com/loudness-subtitle-standards-2026/

## More

- [All datasets](https://shortformkit.com/data/)
- [Free tools for creators](https://shortformkit.com/): downloader, transcripts, LUFS meter, safe zone checker, YouTube money calculator

## License

Data: CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/). Compiled by Shortform Kit (https://shortformkit.com). Every value lists its original source; facts belong to their publishers, the compilation and the CSV/JSON files are CC BY 4.0. Please credit "Shortform Kit, shortformkit.com" with a link.
