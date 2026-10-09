# Digital Media Authenticity, Provenance & Forensics — Advanced Field Guide

**A practical investigation reference for images, video, audio, documents, synthetic media, provenance credentials, source tracing, laboratory workflows and evidence-grade reporting.**

> **Operating principle:** Determine exactly which claim is being tested; preserve the strongest available evidence; prefer original sources and reproducible tests; look for alternative explanations; distinguish verified file integrity from the truth of depicted events. Do not convert detector scores, visual oddities, absent metadata, or archive snapshots into categorical authenticity claims.

<details>
<summary>Contents - all 92 sections</summary>

- [1. Mission and decision model](#1-mission-and-decision-model)
- [2. Case intake and authority](#2-case-intake-and-authority)
- [3. Evidence classes, priority and hierarchy](#3-evidence-classes-priority-and-hierarchy)
- [4. First 10 minutes: field triage SOP](#4-first-10-minutes-field-triage-sop)
- [5. Safe evidence handling and processing environment](#5-safe-evidence-handling-and-processing-environment)
- [6. Universal first-pass command kit](#6-universal-first-pass-command-kit)
- [7. Full acquisition and chain of custody](#7-full-acquisition-and-chain-of-custody)
- [8. Why metadata is contextual, not dispositive](#8-why-metadata-is-contextual-not-dispositive)
- [9. Source discovery and media lineage](#9-source-discovery-and-media-lineage)
- [10. Reverse search operational recipe](#10-reverse-search-operational-recipe)
- [11. Technical image examination: format and structure](#11-technical-image-examination-format-and-structure)
- [12. Image localization: choose tests by hypothesis](#12-image-localization-choose-tests-by-hypothesis)
- [13. Error level analysis (ELA) - correct interpretation](#13-error-level-analysis-ela--correct-interpretation)
- [14. Copy-move, seams, illumination and geometry](#14-copy-move-seams-illumination-and-geometry)
- [15. Sensor pattern noise, CFA and Noiseprint](#15-sensor-pattern-noise-cfa-and-noiseprint)
- [16. AI image detection: defensible use](#16-ai-image-detection-defensible-use)
- [17. Video forensic model: three timelines](#17-video-forensic-model-three-timelines)
- [18. Video container and elementary stream analysis](#18-video-container-and-elementary-stream-analysis)
- [19. Video frame extraction without destroying evidence](#19-video-frame-extraction-without-destroying-evidence)
- [20. Video continuity and manipulation hypotheses](#20-video-continuity-and-manipulation-hypotheses)
- [21. Video codec, GOP and re-encoding analysis](#21-video-codec-gop-and-re-encoding-analysis)
- [22. High-frame-rate, slow motion, interpolation, HDR and generative fill](#22-high-frame-rate-slow-motion-interpolation-hdr-and-generative-fill)
- [23. Video audio extraction and synchronization](#23-video-audio-extraction-and-synchronization)
- [24. Live streams, screen recordings and conference media](#24-live-streams-screen-recordings-and-conference-media)
- [25. Broadcasting and CCTV-specific caveats](#25-broadcasting-and-cctv-specific-caveats)
- [26. Video deepfake detector workflow](#26-video-deepfake-detector-workflow)
- [27. Audio authentication is not just voice-clone detection](#27-audio-authentication-is-not-just-voice-clone-detection)
- [28. Audio intake, codec and continuity](#28-audio-intake-codec-and-continuity)
- [29. Audio waveform and spectrogram workflow](#29-audio-waveform-and-spectrogram-workflow)
- [30. Voice cloning and audio spoofing](#30-voice-cloning-and-audio-spoofing)
- [31. Audio speaker diarization, transcription and language](#31-audio-speaker-diarization-transcription-and-language)
- [32. Audio splice and environment matching](#32-audio-splice-and-environment-matching)
- [33. Voice and video cross-modal checks](#33-voice-and-video-cross-modal-checks)
- [34. Forensic treatment of social-media clips](#34-forensic-treatment-of-social-media-clips)
- [35. Video and audio localization result form](#35-video-and-audio-localization-result-form)
- [36. Documents, screenshots, slides and scanned pages](#36-documents-screenshots-slides-and-scanned-pages)
- [37. PDF and Office quick-read recipes](#37-pdf-and-office-quick-read-recipes)
- [38. OCR and text verification](#38-ocr-and-text-verification)
- [39. AI-generated text: narrow evidentiary scope](#39-ai-generated-text-narrow-evidentiary-scope)
- [40. Content Credentials and C2PA 2.4: correct mental model](#40-content-credentials-and-c2pa-24-correct-mental-model)
- [41. Watermarks, fingerprints and identification](#41-watermarks-fingerprints-and-identification)
- [42. Cross-modal evidence and contradiction matrix](#42-cross-modal-evidence-and-contradiction-matrix)
- [43. Geolocation: validate the event, protect privacy](#43-geolocation-validate-the-event-protect-privacy)
- [44. Chronolocation and event chronology](#44-chronolocation-and-event-chronology)
- [45. Source/circulation provenance graph](#45-sourcecirculation-provenance-graph)
- [46. Reenactment, satire, editorial synthesis and staged content](#46-reenactment-satire-editorial-synthesis-and-staged-content)
- [47. Media authenticity models: laboratory validation protocol](#47-media-authenticity-models-laboratory-validation-protocol)
- [48. Threat models: anti-forensics and inadvertent artifact loss](#48-threat-models-anti-forensics-and-inadvertent-artifact-loss)
- [49. Repeatable SOP A - Viral photo with disputed time/place](#49-repeatable-sop-a--viral-photo-with-disputed-timeplace)
- [50. SOP B - Video alleging a public official said something](#50-sop-b--video-alleging-a-public-official-said-something)
- [51. SOP C - Alleged cloned-voice phone message](#51-sop-c--alleged-cloned-voice-phone-message)
- [52. SOP D - Suspected edited screenshot or forged document](#52-sop-d--suspected-edited-screenshot-or-forged-document)
- [53. SOP E - Suspicious C2PA / Content Credentials claim](#53-sop-e--suspicious-c2pa--content-credentials-claim)
- [54. SOP F - Suspected manipulative short-form video](#54-sop-f--suspected-manipulative-short-form-video)
- [55. SOP G - Fully synthetic or hybrid media in news context](#55-sop-g--fully-synthetic-or-hybrid-media-in-news-context)
- [56. SOP H - Multi-camera reconstruction of a public incident](#56-sop-h--multi-camera-reconstruction-of-a-public-incident)
- [57. SOP I - Public online video with suspected removed/spliced audio](#57-sop-i--public-online-video-with-suspected-removedspliced-audio)
- [58. SOP J - Photo sequence or burst alleged to be “single capture”](#58-sop-j--photo-sequence-or-burst-alleged-to-be-single-capture)
- [59. SOP K - Synthetic text plus counterfeit imagery in coordinated narrative](#59-sop-k--synthetic-text-plus-counterfeit-imagery-in-coordinated-narrative)
- [60. Independent peer review and quality assurance](#60-independent-peer-review-and-quality-assurance)
- [61. Quality gates for high-impact cases](#61-quality-gates-for-high-impact-cases)
- [62. Common misleading arguments and corrections](#62-common-misleading-arguments-and-corrections)
- [63. Practical interpretation patterns](#63-practical-interpretation-patterns)
- [64. Tool and service selection matrix](#64-tool-and-service-selection-matrix)
- [65. Source atlas: core forensic standards, evaluation and provenance](#65-source-atlas-core-forensic-standards-evaluation-and-provenance)
- [66. Source atlas: local file and metadata inspection](#66-source-atlas-local-file-and-metadata-inspection)
- [67. Source atlas: OSINT discovery and publication history](#67-source-atlas-osint-discovery-and-publication-history)
- [68. Source atlas: pixel forensics, manipulation localization and benchmarks](#68-source-atlas-pixel-forensics-manipulation-localization-and-benchmarks)
- [69. Source atlas: audio, speech and video examination](#69-source-atlas-audio-speech-and-video-examination)
- [70. Source atlas: documents, OCR, geospatial and event context](#70-source-atlas-documents-ocr-geospatial-and-event-context)
- [71. Source atlas: commercial/hosted services (access-dependent)](#71-source-atlas-commercialhosted-services-access-dependent)
- [72. A reproducible local evidence-manifest script](#72-a-reproducible-local-evidence-manifest-script)
- [73. A controlled image comparison recipe](#73-a-controlled-image-comparison-recipe)
- [74. A reproducible audio-segment review recipe](#74-a-reproducible-audio-segment-review-recipe)
- [75. Incident/media chronology template](#75-incidentmedia-chronology-template)
- [76. Evidence register template](#76-evidence-register-template)
- [77. Tool execution register template](#77-tool-execution-register-template)
- [78. Source register and citation verification](#78-source-register-and-citation-verification)
- [79. Hypothesis comparison matrix](#79-hypothesis-comparison-matrix)
- [80. Structured finding syntax](#80-structured-finding-syntax)
- [81. Reporting outcome language](#81-reporting-outcome-language)
- [82. Case report skeleton](#82-case-report-skeleton)
- [83. Machine-readable output (optional)](#83-machine-readable-output-optional)
- [84. Open formats and long-term preservation](#84-open-formats-and-long-term-preservation)
- [85. Security when involving LLMs or autonomous agents](#85-security-when-involving-llms-or-autonomous-agents)
- [86. Working with vulnerable populations and sensitive evidence](#86-working-with-vulnerable-populations-and-sensitive-evidence)
- [87. Privacy-aware sample publication](#87-privacy-aware-sample-publication)
- [88. Maintenance and tool-refresh procedure](#88-maintenance-and-tool-refresh-procedure)
- [89. Field checklists by decision stage](#89-field-checklists-by-decision-stage)
- [90. Practical training and tabletop exercises](#90-practical-training-and-tabletop-exercises)
- [91. Final review checklist for this guide](#91-final-review-checklist-for-this-guide)
- [92. Source review notes and provenance](#92-source-review-notes-and-provenance)

</details>

## 1. Mission and decision model

This guide serves OSINT investigators, journalists, verification teams, incident responders, fact-checkers, forensic examiners, attorneys commissioning technical assessments, and authorized security researchers. It is an operational reference, not a substitute for a qualified expert in contested legal proceedings. Apply local evidentiary, consent, privacy, data-retention and disclosure obligations.

**Four separate propositions must never be collapsed:**

| Question | Typical claim | Strongest evidence classes | What it cannot prove |
|---|---|---|---|
| **File integrity** | “These bytes have not changed since acquisition.” | Original-byte SHA-256, signed manifest, custody logs, reproducible comparison | That the source was truthful or the event happened |
| **Provenance/source** | “This originated with camera / publisher / account X.” | Trusted signed origin, first-party original, direct publisher confirmation, corroborating source records | That the scene was unstaged or the speaker consented |
| **Content/context** | “This shows event E at time T in place P.” | Independent event records, reverse-search chronology, environmental/geospatial constraints | Whether all pixels/samples came directly from a sensor |
| **Generation/manipulation** | “AI generated or materially altered this content.” | Validated forensic localization, verifiable creation/edit claims, original-vs-altered comparison, independent technical examination | Who created it or why, absent separate evidence |

The permitted outcome is often **inconclusive**. Do not equate “no visible manipulation detected” with “authentic,” “no C2PA credential” with “fake,” or “contains AI-generated segments” with “the entire recording is synthetic.”

### 1.1 Define the claim before choosing a tool

Write a precise, falsifiable proposition, for example:

- “The published photograph was captured at location L on date D.”
- “The circulating clip is continuous and unedited.”
- “The voice segment from 00:31–00:47 is synthetic.”
- “This PDF existed, unchanged, before the reported event.”
- “The broadcaster's original upload contains the same disputed frame.”
- “The attached JPEG has an intact C2PA manifest signed by a trusted source.”

Specify the alternative hypotheses before looking at results. Examples: ordinary compression; intentional staging; non-AI retouching; transcoding; a captioned older clip; deepfake; an authentically recorded but misleadingly edited sequence; misattribution of a truthful recording.

### 1.2 Five-stage investigation lifecycle

1. **Scope / preserve:** case purpose, legal authority, privacy review, threat model, claim inventory, source acquisition.
2. **Triage / source:** native bytes, metadata, file structure, source discovery, earliest reliable appearances, obvious context checks.
3. **Specialist examination:** modality-specific forensic tests, controls, reference material, detector validation, precise localization.
4. **Correlate / falsify:** compare independent provenance, source, technical, scene and timeline evidence; test alternative explanations.
5. **Peer review / report:** independently reproduce decisive checks, disclose limitations and contradictory evidence, preserve deliverables.

Every test must record: question, prerequisite, source/asset ID, tool/version, command/parameters, output path, observation, interpretation, limitations and what result would overturn the interpretation.

## 2. Case intake and authority

Use a written intake record:

| Field | Required value |
|---|---|
| Case ID | Unique stable identifier |
| Requestor / purpose | Who needs the answer and for what decision |
| Examination questions | Separately numbered testable claims |
| Legal basis / consent | Authority for possessing, processing or sharing media |
| Sensitivity | Public / confidential / regulated / victim content |
| Input sources | Exact URL, sender, device or evidence custodian |
| Acquisition scope | Original file, platform copy, screenshots, logs, embeds |
| Target date range | Event vs publication vs first observation |
| Safety classification | Potential malware, exploit, disturbing content, personal data |
| Sharing restrictions | No-upload, confidential, restricted, internal-only |
| Retention / deletion | Policy and preservation hold |
| Reviewer | Named second examiner or reason unavailable |

**Safety stops:** Do not search for or obtain abusive material involving minors or other unlawful media. Preserve legally held evidence under specialist procedures. Do not identify private people from faces, voices, location clues or nearby personal effects without clear authorization and necessity. Never publicly expose exact private addresses or vulnerable individuals' locations.

### 2.1 Confidence is not probability

Use **high / medium / low confidence** for the quality of an analytical judgment, and separately describe likelihood in ordinary language when supported. No invented numerical certainty. A model output of `0.93` is *a model score*, not automatically a 93% probability that the content is fake.

Record a finding with one of: `VERIFIED`, `SUPPORTED`, `INFERENCE`, `CONFLICT`, `UNRESOLVED`, `NOT TESTED`; add provenance and independence notes.

## 3. Evidence classes, priority and hierarchy

Recommended acquisition order, subject to availability and authorization:

1. Native original from capture device / original file and acquisition metadata.
2. Direct first-party download/API, original publisher's official high-quality rendition.
3. Independently preserved first-party file or verified signed release.
4. Platform-transcoded original post and its metadata.
5. Archive capture of the post or embedded media, preserved with headers/URL context.
6. Reposts, news embeds, screen recordings, screenshots and crops.
7. Descriptions, detector outputs and hearsay about the media.

A screenshot is evidence *of a rendered screen at capture time*; it is not the source JPEG, original video or the underlying document. A public archive is evidence of what that archive captured, not necessarily of the first publication or event date.

### 3.1 Preserve source context

Capture URL (including unshortened final URL where lawful), post ID, handle/account URL, visible timestamp, displayed time zone, retrieval UTC time, captions, comments essential to interpretation, source page HTML or archival capture, media CDN URL, HTTP response metadata, account provenance and redirects. Distinguish third-party embed timestamps from publisher timestamps.

### 3.2 Evidence naming

Use stable IDs rather than descriptions:
`CASE-001-E001-original.mp4`, `CASE-001-E002-platform-copy.mp4`, `CASE-001-D001-trimmed-lossless.wav`. Keep a manifest linking them. Derived artifacts must never overwrite input bytes.

Example case layout:

```text
CASE-001/
├── 00-intake/
├── 01-originals/       # immutable under case procedure
├── 02-acquisition/     # downloaded HTTP metadata, archive captures
├── 03-working-copies/
├── 04-tool-output/
│   ├── metadata/
│   ├── image/
│   ├── video/
│   ├── audio/
│   ├── provenance/
│   └── osint/
├── 05-reference-controls/
├── 06-analysis-notes/
├── 07-peer-review/
├── 08-report/
└── manifest.csv
```

Do not assume ordinary OS file permissions amount to write-blocking or forensic custody. Consider write blockers and storage access logs for evidence-bearing devices. Reading files may alter file-system access times; document your acquisition procedure.

## 4. First 10 minutes: field triage SOP

**Inputs:** exact claim, highest-quality available media, source page.

1. Assign case/asset identifiers; log acquisition and source URL.
2. Hash the acquired byte stream and retain the unmodified copy.
3. Determine actual format using magic bytes, parser reports and file extension. Note mismatches, polyglots and malformed containers.
4. Extract metadata read-only; avoid relying on displayed gallery dates.
5. Identify first-party source and try reverse-image / keyframe searches.
6. Check whether a C2PA credential exists **on this exact rendition**.
7. Inspect obvious contextual mismatches without deciding solely from “AI-looking” details.
8. Enumerate alternative explanations: platform processing, HDR/AI denoising, filters, editorial illustration, editing, old footage.
9. Decide the next test needed to resolve the *specific* claim.
10. Output `CONTINUE`, `REQUEST ORIGINAL`, `SPECIALIST REVIEW`, or `INCONCLUSIVE / NO FURTHER PROPORTIONATE TEST`.

**Escalate immediately** where exposure could cause serious harm, a claim is widely disseminated, source integrity is disputed, a model’s result would be presented as definitive, or a legal decision depends on technical authentication.

## 5. Safe evidence handling and processing environment

Treat every media file, subtitle, browser page, tool repository, embedded link and machine-readable metadata field as **untrusted input**. Media parsers, image previewers and archival viewers can contain vulnerabilities. Use updated inspection tools on isolated systems; do not run supplied scripts, macros, embedded executables or “repair utilities.”

- Work offline with copies for confidential evidence; do not upload victim material, unreleased media or sensitive faces/voices to public detector sites.
- If an online service is used, record terms, data residency, retention, privacy and whether uploads train models or become searchable.
- Use separate low-privilege user accounts, containers/VMs where suitable, restricted outbound network access and allowlisted repositories.
- Pin tool versions/dependencies and record model checkpoint hashes when feasible; consider SBOMs and integrity checks on installed software.
- Do not execute `curl | sh` install scripts on evidence machines.
- Avoid invoking media metadata strings inside unsanitized shell commands or AI-agent tools.
- Test tool behavior on synthetic innocuous samples before handling case data.

## 6. Universal first-pass command kit

The following Bash recipe assumes GNU coreutils on Linux and operates on a trusted working copy. Run in an analysis workspace; adapt paths and installed versions. None of the extraction commands proves authenticity. Replace placeholders only with files you own or are authorized to examine. Each probe records stdout, stderr, exit status and arguments separately; a failed probe does not prevent the remaining checks from running.

```bash
set -eu
FILE="03-working-copies/input-media"
OUT="04-tool-output/metadata"
PROBE_FAILURES=0
mkdir -p "$OUT"

run_probe() {
  local output_name="$1" status
  shift
  printf '%s\n' "$@" > "$OUT/$output_name.argv.txt"
  if "$@" > "$OUT/$output_name" 2> "$OUT/$output_name.stderr"; then
    status=0
  else
    status=$?
    PROBE_FAILURES=$((PROBE_FAILURES + 1))
  fi
  printf '%s\n' "$status" > "$OUT/$output_name.exit-status"
}

run_probe run-time-utc.txt date -u '+%Y-%m-%dT%H:%M:%SZ'
run_probe input.sha256 sha256sum -- "$FILE"
run_probe file-magic.txt file -- "$FILE"
run_probe filesystem-stat.txt stat -- "$FILE"
run_probe exiftool.json exiftool -a -G1 -s -json -- "$FILE"
run_probe mediainfo.json mediainfo --Output=JSON -- "$FILE"
run_probe ffprobe.json ffprobe -v error -show_format -show_streams -of json "$FILE"
run_probe sha256sum-version.txt sha256sum --version
run_probe file-version.txt file --version
run_probe stat-version.txt stat --version
run_probe exiftool-version.txt exiftool -ver
run_probe mediainfo-version.txt mediainfo --Version
run_probe ffprobe-version.txt ffprobe -version

printf 'Failed probes: %s\n' "$PROBE_FAILURES" > "$OUT/summary.txt"
# Return a failure after all probes finish if any command failed.
test "$PROBE_FAILURES" -eq 0
```

`sha256sum` and GNU `stat` are not portable POSIX interfaces; use documented equivalents on other systems. `file`, ExifTool, MediaInfo and ffprobe have partially different coverage; apparent disagreements are investigative leads, not automatic tampering indicators. ffprobe may reject a still image or report limited stream information. Inspect every `.exit-status` and `.stderr` file; an empty or failed output is not a negative forensic result. Use a fresh output directory for each run to retain earlier logs.

For PowerShell:

```powershell
$File = "03-working-copies\input-media"
Get-FileHash -LiteralPath $File -Algorithm SHA256
Get-Item -LiteralPath $File | Format-List *
exiftool -a -G1 -s -json $File | Out-File "metadata.json" -Encoding utf8
mediainfo --Output=JSON $File | Out-File "mediainfo.json" -Encoding utf8
```

Preserve stdout, stderr, return code, full version string and input hash in the method log. Avoid metadata-stripping commands unless processing **a clearly named derivative for publication**, never the evidentiary master.

## 7. Full acquisition and chain of custody

1. Establish whether the source is a camera original, file-system copy, messaging attachment, social-platform output, broadcast stream, archived snapshot or screenshot.
2. Prefer bitstream acquisition of removable media/device where legally authorized and appropriate; preserve file-system metadata and acquisition logs.
3. Record source-provided timestamps verbatim *and* normalized UTC equivalents; specify time-zone assumptions and clock uncertainty.
4. Compute SHA-256 of native evidence immediately after acquisition and again before transfer and reporting.
5. Record acquisition software and settings, redirect chain, HTTP headers, content-disposition, server date and browser version when relevant.
6. Maintain separate identities for: acquired file, archival snapshot, extracted embedded asset, derived transcript, analyzed frame, cropped region and presentation graphic.
7. Export file lists and hashes to a tamper-evident manifest, sign or timestamp if your organization has a validated process.
8. Store originals with restricted access, audit trails and redundant integrity-checked backups.
9. Record each custody event: who, when, why, from/to, medium, hash comparison, condition, authorization.
10. Use an established evidence handling SOP for retention, transfer, court exhibits and deletion.

**Minimal custody record:**

| Case | Asset | Event UTC | Actor | Action | From → To | SHA-256 | Tool | Exception |
|---|---|---|---|---|---|---|---|---|
| CASE-001 | E001 | ISO-8601 | Analyst | Acquisition | Source→Vault | SHA256 | Tool/version | None |

## 8. Why metadata is contextual, not dispositive

EXIF, XMP, IPTC, QuickTime atoms, ID3, PDF Info and filesystem timestamps can be absent, stripped, forged, normalized, copied or generated by software. Camera `Make/Model` is not proof of device ownership. Software tags may indicate export stages but not necessarily that AI was used to generate visual content.

**Probe in this order:**

- Original container type and internal structure.
- Metadata scopes and precedence (embedded tags vs filesystem vs cloud/platform).
- Time-zone, leap-second, daylight-saving and clock-skew issues.
- Edit history, application chains, sidecar files, XMP history where present.
- Embedded thumbnails and previews: compare to principal image.
- GPS with datum/conversion assumptions; inspect whether coordinate precision is plausible.
- Re-encode signatures, color profile, orientation, bit depth and ICC behavior.
- Provenance claims separately from conventional metadata.

**Non-findings:** no EXIF, high ISO without visible grain, perfect-looking skin, odd finger anatomy, unsupported “AI generator” tag or clean spectrogram. Each may prompt another test but does not settle the claim.

## 9. Source discovery and media lineage

Build a **circulation graph** linking each observed rendition to its parent if demonstrable:

`capture → editor/export → publisher → CDN/platform transcode → reupload → screenshot/crop → claim`.

Collect the earliest **reliably dated observed instance**, not simply the oldest search result. A page archive timestamp is an upper bound for availability at that capture, not necessarily the creation time.

Search by:
- Full frame and distinctive crops (avoid over-cropping sensitive people).
- Independent search engines and reverse-image services.
- OCR text on signs and captions, precise quotations, logos, event names and landmarks.
- Keyframes sampled across distinct scenes, not ten nearly identical frames.
- Audio phrase transcripts as **leads**, then corroborate against original recordings.
- Official press libraries, broadcaster archives, creator portfolios and agency media databases.
- Perceptual duplicates (pHash/dHash) as approximate clustering only; verify each result manually.

Log: search engine; query/crop; date/time; result URL; observed media dimensions/hash; relationship; independence; earliest publication evidence; failure/blocked status. Never claim that lack of a reverse-image match implies novelty or synthetic origin.

## 10. Reverse search operational recipe

For an image:
1. Search the untouched original representation.
2. Search a crop of a **distinctive non-personal landmark or object**.
3. Search OCR-extracted visible text exactly and with transliteration.
4. Compare dimensions, crop, watermark, compression and known editorial use.
5. Trace promising hits to their earliest original publisher or license source.
6. Capture result pages while respecting service rules, then verify the media bytes.

For video:
1. Inspect edit structure and scene boundaries.
2. Extract 6–15 diverse frames with timestamps and content hashes.
3. Group visually near-duplicate frames, retain high-information ones.
4. Reverse-search frames and compare them to older reports or footage.
5. Identify whether narration/subtitles are later additions.
6. Compare independent recordings or first-party full-length versions.

**Public search interfaces** may be rate-limited or privacy-invasive for sensitive uploads. Use local approaches or authorized partner channels when appropriate.

## 11. Technical image examination: format and structure

Determine JPEG baseline/progressive, HEIC/HEIF, AVIF, PNG, TIFF, WebP, GIF/APNG, JPEG XL, RAW and proprietary formats. Check:

- Actual magic/header versus extension; truncated or appended data; trailing payloads; embedded object stores.
- Dimensions, color model, alpha channel, ICC profile, orientation transforms and metadata interpretation.
- JPEG quantization tables, sampling factors and coding markers; recognize camera/post-processor defaults can overlap.
- TIFF IFD structure and thumbnail discrepancies; multi-page and layered exports.
- Image rotation/crop, resizing, screenshot/export and platform transcode.
- RAW data and sidecar history, where available; RAW itself may have post-processing or edited previews.
- GIF/APNG frame timing, disposal methods, unexpected frame ordering.
- Pixel-level comparisons **only after aligning color space, orientation, geometric transforms and crop.**

Use multiple parsers for anomalies. A “damaged” file may result from transfer or parser limitations, not intentional alteration.

## 12. Image localization: choose tests by hypothesis

| Hypothesis | Appropriate tests | Mandatory counterchecks |
|---|---|---|
| Region pasted or replaced | Localized compression/noise inconsistency, boundary inspection, segmentation maps | Different textures/illumination, in-camera HDR, selective denoise |
| Region duplicated | Copy-move nearest-neighbor/feature matching, transformed patch correlation | Repeating architectural patterns, vegetation, water, design templates |
| Entire image synthesized | Model benchmark(s) on matched controls; available signed generation assertion; source search | Real images edited with AI enhancement; unseen camera/codec domain |
| Object removed | Source-original comparison, patch inconsistencies, semantic/contextual gaps | Legitimate object movement, crop, blur, content-aware editorial edit |
| Context miscaptioned | Reverse search, scene geography, chronology, weather, event records | Time-zone differences, older images reused for legitimate illustration |
| Device attribution disputed | Sensor-specific PRNU under controlled reference conditions | Multiple devices with same model, crop, denoise, recompression, references not independent |

**No single image heatmap is proof of manipulation.** Localization is a *model output* requiring controls and review.

## 13. Error level analysis (ELA) — correct interpretation

ELA highlights differences after recompression under chosen settings. It is highly sensitive to JPEG quality, existing compression, local contrast, repeated saving, color profiles, subsampling, added text and re-encoding.

Operational conditions:
1. Determine whether input is actually JPEG, not a screenshot re-encoded from PNG or an image previously saved repeatedly.
2. Record recompression quality and subsampling, decoder and all preprocessing.
3. Compare with **matched negative controls**: authentic screenshots, photos, images with legitimate overlays, images with repeated compression.
4. Compare suspect and non-suspect regions of similar texture and luminance.
5. Review independent evidence rather than giving binary “red means edited” answers.
6. If the original is PNG or severely compressed, treat ELA as unlikely to be diagnostic.

**Prohibited conclusion:** “bright ELA region proves Photoshop/AI.” Better: “recompression residuals differ in region R under settings S; several non-malicious processing paths remain plausible.”

## 14. Copy-move, seams, illumination and geometry

- Perform feature-based or block-based duplicate search on **aligned** versions; record scale, rotation, tolerance.
- Exclude ordinary repetitive scenes by inspecting long-range spatial context.
- Examine perspective, vanishing points, occlusion order, edge quality, shadow geometry and reflections as independent scene constraints.
- Account for multiple light sources, HDR stacking, flash, glass, mirrors, wide-angle distortion and rolling-shutter effects.
- Use photogrammetry when calibrated reference geometry is available; report propagated measurement uncertainty.
- Do not use anatomy/gaze/“uncanny valley” as calibrated proof. Modern synthetic content may show none of the old defects, and genuine footage may look unusual.

## 15. Sensor pattern noise, CFA and Noiseprint

**PRNU (photo-response non-uniformity)** is a device-associated sensor pattern extracted from multiple suitable reference photos under specific conditions; it is not synonymous with visible grain. Camera-model traces (e.g., Noiseprint) are different from device-level identification.

Expert workflow:
1. Acquire multiple genuine, independent reference images from the **claimed device** where authorized.
2. Match resolution, processing pipeline, lens/orientation and sensor crop as closely as possible.
3. Avoid highly textured, saturated, clipped and heavily compressed areas where residuals are unreliable.
4. Apply a validated residual estimator and correlation statistic to held-out control material.
5. Estimate false-match behavior for other devices, the same camera model and edited/transcoded derivatives.
6. Record reference selection bias, unknown intervening transformations and thresholds.
7. Report support for/against a source hypothesis; never infer a person's identity from noise alone.

Camera-model fingerprinting, CFA/demosaicing and chromatic aberration tests can be invalidated by resizing, computational photography, AI denoise, multi-frame fusion and post-processing. Document exactly which pipeline assumptions hold.

## 16. AI image detection: defensible use

Specify the model/checkpoint, model card, dataset, date, operating threshold, supported image range and preprocessing. Evaluate at least:
- Held-out **real** images from relevant phones, cameras and editorial workflows.
- Synthetic samples from **unseen generation families** and editing models.
- Platform screenshots, reuploads, crops, resizing, JPEG/webp recompression, filters and watermark overlays.
- Different languages/context and photography genres where relevant.
- Blended images with only a small synthetic region.

Measure confusion matrix, sensitivity, specificity, precision at the expected base rate, FPR at chosen threshold, ROC/PR curves, reliability/calibration, subgroup/domain performance, abstention rate and uncertainty. Avoid leakage between train/validation/test from near-duplicate parent media.

**Model disagreement is informative about uncertainty, not a democratic vote.** Three detectors trained on the same dataset or architecture do not constitute three independent lines of evidence.

Research frameworks such as TruFor, DeepfakeBench and Noiseprint are **not automatically validated casework instruments**. Validate and document them within your own setting before drawing high-stakes conclusions.



## 17. Video forensic model: three timelines

Maintain three distinct timelines:
1. **Media presentation:** decoded presentation timestamps (PTS) and sound intervals.
2. **Capture / device:** camera clock, recording start/stop and alleged source sequence.
3. **External events:** incident timeline supported by independent records.

Time-base, variable-frame-rate conversion, B-frames, edit lists, slow motion, pause/resume and social-platform transcoding can make the three timelines diverge. A frame index divided by nominal FPS is not necessarily an exact elapsed time.

## 18. Video container and elementary stream analysis

Inspect ISO BMFF/MP4/QuickTime, Matroska, MPEG-TS, AVI, WebM and proprietary formats:
- Container metadata vs actual video/audio streams.
- Codec profile/level, color primaries, transfer characteristics, mastering/HDR metadata and variable frame rate.
- Stream count, chapters, edit lists, timescales, duration, track start offset and rotation.
- GOP/keyframe pattern, changes in frame size, bitrate, frame timing and encoding parameters.
- Audio and video clock behavior and potential resynchronization.
- Subtitle/data tracks, overlays, logos and timecode streams.
- Truncation, interrupted recording, discontinuities and parser recovery.
- Broadcast timecodes, media server transcodes, OBS/screen-recording artifacts.

Example read-only probes:

```bash
ffprobe -v error -show_format -show_streams -of json "input.mp4" > streams.json
ffprobe -v error -select_streams v:0 \
  -show_entries frame=best_effort_timestamp_time,pkt_duration_time,key_frame,pict_type \
  -show_frames -of csv=p=0 "input.mp4" > video-frames.csv
ffprobe -v error -select_streams a:0 \
  -show_entries packet=pts_time,dts_time,duration_time,size \
  -show_packets -of csv=p=0 "input.mp4" > audio-packets.csv
mediainfo --Full "input.mp4" > mediainfo-full.txt
```

`best_effort_timestamp_time` and packet fields can be missing or parser-dependent; record limitations. Output can be very large—use representative subsets for case exhibits, retain full raw output separately.

## 19. Video frame extraction without destroying evidence

Decoding frames creates **derived evidence**. Name frames with their source PTS/timecode where practical; don't mistake extracted PNG creation time for capture time.

```bash
mkdir -p derived/keyframes derived/scenes derived/frames
# Preserve every decoded video frame as lossless PNG — potentially very large:
ffmpeg -hide_banner -i "input.mp4" -map 0:v:0 -vsync 0 \
  "derived/frames/frame_%08d.png"
# Uniform sampling for search/triage only:
ffmpeg -hide_banner -i "input.mp4" -vf "fps=1/2" \
  "derived/keyframes/each_2s_%05d.png"
# Scene-change candidates; adjust threshold after checking trial results:
ffmpeg -hide_banner -i "input.mp4" \
  -vf "select='gt(scene,0.35)'" -vsync vfr \
  "derived/scenes/scene_%05d.png"
```

**Important:** The `-vsync` option may be deprecated or differ across FFmpeg versions; inspect `ffmpeg -h full` and prefer current equivalent behavior when available. Uniform sampling duplicates/drops temporal information and must never be used to infer continuity. If VFR is central to the claim, export precise frame timestamps and retain original stream.

## 20. Video continuity and manipulation hypotheses

Test for:
- Missing or repeated spans; insertion, reordering, speed changes and discontinuities.
- Cross-frame identity/appearance inconsistency; but avoid automated person identification.
- Optical-flow jumps, object motion inconsistency, camera-motion discontinuities.
- Edge artifacts in face swaps, temporal warping, occlusion failures, compositing seams.
- Compression/resolution/color profile changes across time.
- Audio-video desynchronization and lip movement mismatch.
- Background lighting/shadow changes, weather and object permanence.
- Deepfake/CGI artifacts that may vary by scene or degradation.

**Counterexplanations:** camera pause/resume; VFR and B-frame reordering; stabilization; teleconferencing effects; automated subtitles/virtual backgrounds; jump cuts; archival splice in legitimate news reporting; network packet loss; rolling shutter; frame interpolation; platform recompression; HDR tone mapping.

For each flagged segment record `start PTS`, `end PTS`, frame IDs, evidence class, alternative and confidence. Review at original speed and frame by frame with the source audio.

## 21. Video codec, GOP and re-encoding analysis

Codec anomalies can corroborate editing **only after modeling the recording and export pipeline**. Compare:
- Scene-by-scene frame sizes/bitrate distribution and GOP structure;
- keyframe insertion from scene cuts;
- metadata about encoder application and conversion histories;
- inconsistent quantization, macroblock boundaries or chroma sampling;
- embedded timestamps and camera file-segmentation conventions;
- scene changes versus forced I-frames;
- video/audio track origin discrepancies.

Avoid claims that “two compression levels = forgery.” Legitimate mobile cameras, messaging apps, social platforms and video editors alter these features.

## 22. High-frame-rate, slow motion, interpolation, HDR and generative fill

Check capture rate vs playback FPS, optical flow interpolation, depth-of-field simulations, temporal super-resolution, AI frame generation and HDR blending. Slow motion can make lip movement appear artificial; motion-compensated interpolation can synthesize intermediate frames without changing underlying event authenticity. Document both editorial alteration and whether it materially affects the disputed claim.

## 23. Video audio extraction and synchronization

Preserve original streams and separately create analysis derivatives:

```bash
mkdir -p derived/audio
# Extract original first audio stream without transcode when compatible:
ffmpeg -i "input.mp4" -map 0:a:0 -c copy "derived/audio/stream.m4a"
# Analysis-only PCM WAV; changes representation but not equivalent to raw original:
ffmpeg -i "input.mp4" -map 0:a:0 -vn \
  -acodec pcm_s24le "derived/audio/analysis.wav"
# Analyze timing:
ffprobe -v error -select_streams a:0 \
  -show_packets -show_entries packet=pts_time,duration_time -of csv=p=0 \
  "input.mp4" > derived/audio/packet-timing.csv
```

**Note:** `-c copy` requires compatible output container; select output extension based on actual input codec (e.g. `.aac`, `.m4a`, `.opus`, `.mka`). Do not assume sample-accurate synchronization after conversion. Preserve offset information. Generate synchronized diagnostic playback if lip sync is questioned, and note playback-device latency and time stretching.

## 24. Live streams, screen recordings and conference media

Distinguish a live event from its recording, stream packaging, subsequent clipping and on-screen representations. Review HLS/DASH playlist, segment boundaries, discontinuities, transcoding tiers and player overlays when lawfully collected. Screen captures can show synthetic avatars, AI noise reduction, filters or virtual camera effects even when meeting participation is genuine. Never conclude that a depicted person was physically present solely from a video conference image.

## 25. Broadcasting and CCTV-specific caveats

- CCTV clocks often drift; validate against independent clocks and system/NVR logs when accessible.
- Proprietary exports may include player-dependent metadata or watermarks; request native export plus proprietary player and independent decoded copy.
- Watermark, channel logo or timecode is not automatically cryptographically authenticated.
- Broadcast rebroadcast/recompression can produce mismatched fields and ghosting.
- Interlacing, deinterlacing and scaling affect apparent objects and positions.
- Camera blind spots, lens distortion, PTZ movement and video analytics overlays alter scene appearance.
- Streaming surveillance exports may omit gaps; request recording/event indexes where authorized.

## 26. Video deepfake detector workflow

1. Define manipulation class: face-swap, reenactment, lip-sync edit, generative full scene, synthetic avatar or merely AI upscaling.
2. Establish whether detector supports that class, codec, resolution, face size and frame count.
3. Select representative segments including suspected and apparently normal frames.
4. Run on a **matched set of authentic reference footage** undergoing the same compression/transcoding, ideally from the same source workflow.
5. Record per-frame scores, aggregate rule and confidence intervals; avoid treating sampled frames as independent observations.
6. Correlate localized anomalies with timing/context and source-original differences.
7. Test failure modes: motion blur, side profiles, occlusions, dark skin tones, low light, heavy makeup, low bitrate and split-screen.
8. Have a second analyst review without prior conclusion.

**Do not** equate detector-reported “face authenticity” with whether the speaker actually said the alleged words. Lip-sync analysis requires corresponding audio provenance.

## 27. Audio authentication is not just voice-clone detection

Separate five questions:
- Is the **audio file structure** compatible with alleged recording conditions?
- Was the recording **edited or spliced**?
- Is the speech **synthetic or voice-converted**?
- Is the apparent **speaker identity** supportable from authorized independent evidence?
- Are the **spoken claims** genuine and properly contextualized?

A genuine recording may contain edited speech. A cloned voice may read a true quotation. A real speaker may speak through synthetic denoising or live enhancement. Do not conflate these.

## 28. Audio intake, codec and continuity

Record original WAV/BWF, AIFF, FLAC, MP3, AAC, Opus, AMR, OGG or phone/voicemail exports; note channel count, bit depth, sample rate, encoder metadata and phone-network artifacts. Check:
- DC offset, clipping and silence distributions;
- channel phase/cross-correlation and asymmetry;
- gain jumps and equalization discontinuities;
- changes in noise floor, ambience or reverberation;
- music beds, speech overlays, conferencing noise suppression and automatic gain control;
- compression/generation artifacts and codec boundaries;
- sample discontinuities and edited word boundaries;
- timestamps and sample counts where trustworthy.

Never call a frequency cutoff or “clean breath” proof of synthetic audio: narrowband phone codecs, lossy encoders and denoise systems create similar signatures.

## 29. Audio waveform and spectrogram workflow

Use Audacity, Sonic Visualiser, Praat or a controlled Python environment:
1. Listen at original speed; transcribe disputed words only as a **draft**.
2. Inspect waveform and spectrogram at multiple scales, with STFT window/hop size documented.
3. Zoom around claimed splice boundaries and background noise changes.
4. Compare overlapping segments for exact repeated samples (separate copy-paste from naturally repeated words).
5. Evaluate reverberation, spectral tilt, harmonic structure, clipping, frequency response and room/codec changes.
6. Assess pauses, plosives, sibilants, breaths, fricatives, phase discontinuity and coarticulation while noting normal variability.
7. Review potential automatic noise gates, limiter pumping, enhancement filters and podcast mastering.
8. Create a timestamped segment list; store original and derived waveforms separately.

Example reproducible visualization as a **local derivative**:

```bash
mkdir -p derived
ffmpeg -i "audio-source.m4a" \
  -filter_complex "[0:a:0]showspectrumpic=s=1600x900:legend=1[spectrum]" \
  -map "[spectrum]" -frames:v 1 "derived/spectrogram.png"
# Do not use filters on the evidentiary master; store all derivatives separately.
```

Check your FFmpeg build supports the chosen filter/options.

## 30. Voice cloning and audio spoofing

Relevant detector families: waveform models, log-Mel spectrogram classifiers, self-supervised speech embedding classifiers, anti-spoof models and ensemble systems. Require an **independent held-out benchmark** and matched controls.

Additional confounders: accent, non-English languages, whispered/sung/shouted speech, playback over speakerphone, phone compression, re-recorded audio, speech enhancement, voice disorder, laughter, emotion, age and microphones. Some synthetic speech is generated without mimicking a specific person.

An anti-spoofing score is not proof of who spoke. **Speaker recognition is a separate specialist task** that may require a consent-based reference set and expert evaluation; do not conduct intrusive identification of private individuals from incidental voice samples.

ASVspoof5 provides research baselines and evaluation protocols; evaluate generalization before any case-level inference. An equal-error rate reported on a research dataset is not an on-site false-positive rate.

## 31. Audio speaker diarization, transcription and language

Diarization (“who spoke when,” assigning *anonymous* speaker labels) and transcription help navigate long recordings, but both introduce errors. Use local Whisper/whisper.cpp or other ASR only for indexed leads and revise manually against the original. Record uncertain words and overlapping speech. Machine translation can alter implication, idiom and legal meaning; use qualified translators for contested utterances.

Keep:
- original timestamps and speech intervals;
- diarization model/version and anonymous labels;
- ASR transcript with confidence/uncertainty notes;
- analyst-corrected transcript with provenance;
- translation and translator qualifications if material;
- contradictory alternative hearings.

Synthetic speech may be **partially replaced at a word or phoneme level**. Do not classify only at whole-file granularity.

## 32. Audio splice and environment matching

For a claimed continuous recording, compare:
- ambient bed/noise floor across cuts, excluding naturally changing sound;
- room impulse and echo patterns;
- electrical interference, mains hum where actually present;
- microphone response, AGC and compressor pumping;
- overlapping speech/background event continuity;
- codec packets, silence padding and edit boundaries;
- isolated syllable inconsistencies against matched examples.

Avoid treating room acoustics as immutable: moving people/phones, doors and different microphone modes change acoustic response.

## 33. Voice and video cross-modal checks

Check speech-to-lip alignment in **PTS**, not guessed FPS; voice timbre versus ambient environment; gesture/speech naturalism; visible objects making sound; subtitles versus audio. Account for dubbing, simultaneous interpretation, delays, streaming jitter, video edits, accessibility captions and voice-over. A mismatch supports a synchronization/editing hypothesis, not automatically AI synthesis.

## 34. Forensic treatment of social-media clips

Always distinguish:
- locally acquired or original media;
- platform delivery version and transcoding profile;
- in-app filter effects;
- reuploads, stitched/remixed clips, reaction videos and duets;
- burn-in captions, watermarks and sticker layers;
- automatic platform-generated subtitles/translation;
- recommendation/feed context and later caption edits.

Platforms may use multiple CDN representations; downloads made at different times or account settings need not be byte-identical. Preserve both URL-level provenance and byte hashes of each rendition.

## 35. Video and audio localization result form

| Segment | Media time | Claim tested | Observed artifact | Method / controls | Non-malicious explanation | Judgment |
|---|---|---|---|---|---|---|
| S001 | 00:24.510–00:27.100 | Possible splice | Ambient bed change | Spectrogram + independent original | Microphone/AGC switch | Unresolved |
| S002 | 01:12.050–01:13.120 | Visual synthesis | Frame-local anomaly | Detector + matched controls | Scene compression | Needs expert review |

Do not publish such rows as demonstrated factual case findings; this is a **blank illustrative pattern**, with invented example values.

## 36. Documents, screenshots, slides and scanned pages

A document may be generated by AI, edited, composited into a screenshot, or simply misattributed. Treat these as different tests.

**Native file investigation:**
- PDF object catalog, XRef tables, incremental updates, embedded files, font subsets, metadata and signatures.
- DOCX/XLSX/PPTX as ZIP/OOXML package: core/custom properties, media, relationships, tracked changes, comments, revisions and hidden sheets/slides.
- Print-to-PDF and image-scan workflows can erase source-edit history.
- Digital signature validation must include certificate chain, trust policy, signing time and revocation status where applicable.
- Fonts, layout artifacts and OCR mistakes are not generator fingerprints without controls.

**Screenshot investigation:**
- Verify whether claimed interface existed at that date/version and platform.
- Inspect status bars, page locale, dark mode, fonts, responsive layout and browser chrome.
- Compare with official webpage/email/account exports (authorized) and historical captures.
- Check cropped context, coordinate scaling, overlays and edited regions.
- Avoid assuming screenshot EXIF describes the underlying document or website.

**Document text content:**
- Verify citations, legal filings, quotations and URLs against originals.
- Machine-written style is not conclusive proof of AI assistance.
- Exact duplication, document revision history or verified disclosure may be much stronger than prose stylometry.

## 37. PDF and Office quick-read recipes

Read-only tool entry points, after testing in a sandbox and checking syntax:

```bash
pdfinfo "document.pdf" > derived/pdfinfo.txt
qpdf --check "document.pdf" > derived/qpdf-check.txt 2>&1
exiftool -a -G1 -s "document.pdf" > derived/pdf-metadata.txt
# List, but do not execute, the members of an OOXML archive:
unzip -l "document.docx" > derived/ooxml-contents.txt
# Work on a disposable copy only if extracting embedded media or XML.
```

**A valid `qpdf --check` result indicates parser/structure checks passed**, not document truth or signature validity. Some PDF parsing operations can behave differently on encrypted, malformed or linearized files; log warnings.

For signed documents, use appropriate platform-specific signature tooling and PKI expertise. Do not use generic PDF metadata as a substitute for cryptographic validation.

## 38. OCR and text verification

Tesseract, PaddleOCR, OCRmyPDF and document layout parsers produce **derived OCR interpretations**, not the source. Retain the scan and record page coordinates, language models and preprocessing. Check numbers, decimal commas, dates, names, letterforms, stamps and low-contrast regions manually. OCR hallucinations can create false names and citations. Do not infer document authenticity from grammatical quality or apparent typography alone.

## 39. AI-generated text: narrow evidentiary scope

General-purpose AI-written text detection can be unreliable, especially for short passages, non-native English, translation, heavy edits, templated professional prose and domain shifts. Avoid numerical "AI percent" verdicts. Prefer verifiable provenance: draft/revision record, authenticated publishing logs, direct writer disclosure or file history. Stylometry may support an authorship comparison only with representative, consented reference texts and rigorous evaluation.

## 40. Content Credentials and C2PA 2.4: correct mental model

C2PA uses signed, cryptographically bound claims about digital assets and editorial actions. The **trust model is primarily about a signing identity and integrity of signed assertions**; it does not automatically prove the underlying factual truth of a scene.

Spec 2.4 (April 2026) includes new `c2pa.ai-disclosure`, `c2pa.repository-receipt` and sustainability assertions, plus a derived `crJSON` representation. `crJSON` is a **derived export, not a canonical independently verifiable source**. Interpret explicit AI disclosures based on exact assertion semantics and signer's trustworthiness, not as a universal fake/authentic verdict.

### 40.1 Always separate five tests

1. **Presence:** Does this exact asset have embedded/sidecar/discoverable credentials?
2. **Binding:** Does a manifest cryptographically bind to this exact file or represented rendition?
3. **Signature:** Does the cryptographic validation of the claim succeed?
4. **Trust:** Is the signer accepted under the investigative trust policy / relevant trust list, at relevant time?
5. **Claims:** What exactly does the signer assert about actions, ingredients, AI or capture? Is external corroboration available?

A valid signature does **not** mean every descriptive assertion is true. Absence of credentials is not evidence of fabrication. A screenshot of a Content Credentials verification badge is not a substitute for re-verifying the actual asset.

### 40.2 Offline CLI triage

```bash
c2patool --version
c2patool "03-working-copies/input-media" > \
  "04-tool-output/provenance/c2pa-report.json"
```

Check current `c2patool --help` for low-level or trust validation options, JSON output modes, policy configuration and supported formats. Always save stderr, exit status and version. A mere readable manifest is not evidence of successful trust validation. Do not use signing/embedding subcommands on evidence.

### 40.3 Failure matrix

| Finding | Possible meaning | Next step |
|---|---|---|
| No manifest | Never issued, stripped by platform, unsupported format, broken embedding | Check first-party original or associated manifest store |
| Invalid asset binding | Asset changed, corrupted, mismatched or incorrectly serialized | Re-check exact bytes and validator details |
| Signature valid, signer untrusted | Cryptography passed but policy trust absent | Evaluate signer independently, trust-list validity and policy |
| Trusted signature, implausible event | Claims may be false or scene staged | External scene/context corroboration |
| Trusted capture with later AI edit | Mixed real/synthetic workflow | Inspect action/ingredient graph and exact edited regions |
| Manifest present only as JSON export | Possibly a report rather than verifiable signed manifest | Validate original signed structure, not only JSON |
| Credential lost after export | Platform/editor stripped or changed embedding | Preserve chain through earlier asset versions; do not invent missing steps |

### 40.4 Identity and privacy

Signers are not necessarily natural persons; signatures may belong to cameras, software or organizations. Signed assertions may disclose identity data. Redact selectively in public reports while preserving originals in restricted evidence storage. Do not infer real-world private identities from signing identifiers without documented authorization.

## 41. Watermarks, fingerprints and identification

Distinguish:
- visible logo/branding (easy to copy);
- invisible watermark embedded in pixels/audio or model output;
- perceptual fingerprint identifying near duplicates;
- cryptographic hash identifying an exact byte sequence;
- C2PA hard binding verifying bytes/covered ranges;
- soft binding used for rendition matching/recovery.

Access to proprietary watermark verification (e.g., certain generative-model watermarks) may be restricted. A negative test with an unsupported detector is `NOT TESTED`, not evidence of watermark absence. Watermarks can be altered by transformations; spoofing and false positives must be considered.

## 42. Cross-modal evidence and contradiction matrix

Maintain independent lanes:

| Lane | Input | Evidence | Main error mode |
|---|---|---|---|
| Bytes | Original file | Hash, structure, technical headers | Acquired wrong rendition |
| Signed provenance | Embedded or detached manifest | Verified binding/signature/trust | Trust conflated with factual truth |
| Publication | Publisher and archives | First observed URL/time | Archive time conflated with event |
| Scene | Environment, geometry, objects | Independent geographic/temporal corroboration | Reenactment / historical imagery |
| Model | Validated detector | Scores, localization, controls | Dataset/domain shift |
| Human witness | First-person, authenticated testimony | Context/supporting account | Memory, incentives, misidentification |
| External event | Official records and independent reports | Event corroboration | Circular reporting and copied claims |

Never treat two news outlets quoting the same statement as independent corroboration. Keep source lineage explicit.

## 43. Geolocation: validate the event, protect privacy

For public-interest events, prioritize venue, landmark, terrain, road geometry, sunlight orientation, skyline, street furniture and historical map state. Compare:
- OpenStreetMap and map imagery licensing/timestamp;
- street-level imagery **capture date** and possible removals;
- satellite imagery acquisition date, seasonality and resolution;
- terrain and mountain skyline;
- directional signs, road markings, transit signage;
- construction and demolition chronology;
- shadows, compass heading and camera projection;
- weather and atmospheric/haze constraints.

**Do not** reconstruct private residences, minor locations, vulnerable persons' shelters or precise live routes from incidental media. Generalize output to the minimum precision needed.

## 44. Chronolocation and event chronology

Maintain separate columns for:
- alleged event local time, with uncertainty;
- recording device clock and offset;
- EXIF/QuickTime date;
- uploader’s claimed publish time;
- platform first-seen time;
- archive crawl/capture time;
- independent external record time;
- analyst collection time UTC.

Use uncertainty intervals rather than a forced exact timestamp. Shadow measurements can suggest ranges under known camera geometry, location and lighting conditions; artificial or multiple lighting sources break simplistic calculations.

Weather, clouds, snowfall, tides, visible moon/stars, public schedules and construction dates are complementary constraints. Confirm quality/spatial resolution of underlying records before relying on them.

## 45. Source/circulation provenance graph

Store graph edges with timestamp, evidence and relationship type:
- `COPIED_FROM` where demonstrated by same file, signature or publication provenance.
- `DERIVED_FROM` where edits/crops/transcodes are demonstrable.
- `EMBEDS`, `LINKS_TO`, `CITES`, `CLAIMS_SAME_EVENT_AS` (not proof of derivation).
- `PUBLISHED_BY` only where the publisher/account is verified.
- `ALLEGED_SOURCE` for unverified attributions.

Track *first seen*, not confidently *first published* unless substantiated. Search and archive results have incomplete coverage.

## 46. Reenactment, satire, editorial synthesis and staged content

A genuine camera recording can show a scene staged specifically to mislead, and an AI-generated illustration can accurately describe a real news event. Report separately:
- whether the media is synthetic/edited;
- whether it is labeled satire, illustration, reenactment or archival;
- whether the caption/context makes a false factual claim;
- whether a recipient would reasonably mistake it for event footage;
- whether consent/disclosure considerations arise.

This avoids the false dichotomy `real pixels = true story` / `synthetic pixels = false story`.



## 47. Media authenticity models: laboratory validation protocol

Before deploying any automated classifier or localization model, complete a **model acceptance worksheet**. At minimum record:
- research question and class definition (AI generated, altered, splice, source camera, document authorship);
- version, weights checksum, license, developer, input requirements and system environment;
- training dataset provenance, subject overlap, platform/codec and geographic/language coverage;
- holdout datasets and **near-duplicate disjointness** by source;
- augmentation and preprocessing (crop/resize/color conversion, enhancement, face detection);
- class imbalance and realistic operational prevalence;
- decision thresholds set *before* the holdout test;
- measurement units (file, segment, face track, frame, region, session);
- control comparisons with genuine edited media and AI-enhanced legitimate media;
- no-match / out-of-distribution detection and abstention behavior;
- calibration method and domain-shift tests;
- privacy, data retention, external-network behavior and consent.

### 47.1 Evaluate appropriate metrics

| Metric | Definition / use | Common trap |
|---|---|---|
| TPR / sensitivity | TP / (TP+FN) | Overstates utility when false positives costly |
| FPR | FP / (FP+TN) | Tiny FPR on small sample is unstable |
| Specificity | TN / (TN+FP) | Requires representative negatives |
| Precision / PPV | TP / (TP+FP) | Changes with base rate |
| Recall | TPR | Not distinct from sensitivity |
| ROC-AUC | Ranking across thresholds | Good AUC does not guarantee useful operating point |
| PR-AUC | Precision-recall tradeoff | Depends on prevalence |
| EER | Point where FNR≈FPR | Benchmark property, not case probability |
| Brier score / ECE | Calibration quality | Needs suitable probability estimates |
| Localization IoU / Dice | Overlap of predicted vs ground-truth region | Requires trustworthy labels |
| Segment F1 | Correct altered interval detection | Boundary tolerance must be stated |
| Abstention coverage / risk | How often tool declines judgment | Hiding hard cases improves apparent accuracy |

**Base-rate example (illustrative, not a product claim):** a detector at 95% sensitivity and 5% FPR, when only 1% of a batch is fake, yields PPV ≈ `(.95×.01)/(.95×.01 + .05×.99) = 16.1%`. Therefore an apparently excellent detector can still generate mostly false alarms in low-prevalence screening.

Never transform benchmark AUC, vendor marketing accuracy or a single detector score into a forensic likelihood ratio. For population or court-use likelihood ratios, specialist statistical calibration and validated populations are needed.

### 47.2 Paired degradation study

Create a benign, rights-cleared control set containing:
- sensor-native photos and video; genuine photos with legitimate retouching;
- real screenshots, compressed messaging copies, broadcast and teleconference recordings;
- disclosed synthetic examples from several *unseen* model families;
- local edits and composite regions with known ground truth;
- audio generated/recorded with known disclosure, plus telephone and noise-suppressed derivatives.

Generate derivative variants at fixed operations: JPEG quality series, WebP, AVIF, resize, crop, rotate, overlay text, screen recording, blur, stabilization, re-encoding, stereo/mono, Opus/MP3 conversion, resampling, reverberation, music overlay. Hold provenance labels constant and measure detection drift. Record transform order because it matters.

### 47.3 Model reproducibility

Store `model_id`, repository commit, checkpoint SHA-256, dependency lock, hardware architecture, input normalization, random seed, inference batch and runtime logs. A heatmap screenshot without the underlying model build and raw output is insufficient.

### 47.4 Ensemble independence

Before combining two detectors, determine whether they share training data, same feature extractor, same model lineage or overlapping negative controls. Correlated errors must not be multiplied as if independent likelihoods. A model ensemble may add robustness but does not by itself amount to independent factual corroboration.

## 48. Threat models: anti-forensics and inadvertent artifact loss

| Mechanism | Possible effect | Defensive analyst response |
|---|---|---|
| Metadata spoofing | False capture time/device or editor history | Corroborate outside file |
| Screenshot laundering | Hides source media structure | Request native bytes; report screenshot-only limit |
| Recompression / upscaling | Removes or distorts forensic traces | Source lineage and transform-matched controls |
| Generative inpainting | Small synthetic region inside authentic image | Region hypothesis and original comparison |
| Adversarial detector targeting | Detector outputs deliberately altered | Model diversity, OOD testing, source records |
| C2PA manifest stripping | Credentials absent from rendition | Seek earlier signed asset; no inference from absence |
| Trust / signer spoofing | Misleading display names or untrusted certificates | Cryptographic and trust validation |
| Synthetic audio re-recording | Playback introduces room acoustics | Multiple acoustic/codec checks, original request |
| Voice conversion on genuine speech | Identity timbre changed, words may be genuine | Separate utterance authenticity from identity |
| Deepfake over real event | False subject/action added to real context | Compare independent footage or source frames |
| Timecode injection | Apparent timestamp without verified clock | Independent clock and recording chain |
| Coordinated false-source sites | Circular corroboration | Identify common source lineages and independent records |

Describe indicators and defensive tests; do not treat this table as a recipe for fabricating undetectable evidence.

## 49. Repeatable SOP A — Viral photo with disputed time/place

**Goal:** determine whether a viral photo depicts the stated event at the claimed time/place.

1. Record original post, claim, exact visible text and initial UTC collection.
2. Acquire highest-quality available image and source page; hash and log variants.
3. Search image and landmark crops through several reverse-search services.
4. Find earliest verifiable publication(s), licensing/stock sources and original captions.
5. Compare scene against historical imagery and construction timelines.
6. Verify weather/season/lighting only after establishing plausible location and camera orientation.
7. Examine file metadata and compression for process history, but do not equate absent EXIF with AI.
8. For potential local manipulation, define exact area and test with matched controls and manual alignment.
9. Seek independently dated visual corroboration from the same event.
10. Produce timeline with separate capture/publish/archive dates and alternative explanation.
11. Report whether **claim context** is supported, independent of media-generation classification.
12. Peer-review the decisive geolocation and earliest-publication links.

**Deliverables:** image hash, source graph, exact URLs, comparison panel with source attribution, geospatial constraints, chronology, confidence and gaps.

## 50. SOP B — Video alleging a public official said something

1. Define disputed utterance with exact interval and transcript.
2. Acquire full first-party performance/broadcast if available; preserve clip and full stream separately.
3. Hash copies; obtain container and stream metadata.
4. Extract timestamp-preserving audio and frames, keeping transformation logs.
5. Compare the disputed clip against authorized full-length source at frame/audio level.
6. Check lip-sync with timing/stream-offset adjustments, unrelated overlays, edits and dubbing.
7. For suspected synthetic voice, evaluate independent audio spoof methods on representative reference controls.
8. For face manipulation, use model and manual review on matched compression.
9. Corroborate the event schedule, official transcripts and contemporaneous reporting without treating repeated summaries as independent sources.
10. Assess alternative possibilities: authentic quotation cut out of context, edited transcript, translation/dubbing, deliberate reenactment, AI alteration.
11. Redact incidental private individuals in publication derivatives.
12. Publish careful claim-specific assessment, not a diagnosis of personal identity or motives.

## 51. SOP C — Alleged cloned-voice phone message

1. Preserve native voicemail/telephony export plus platform/account metadata where lawfully provided.
2. Note whether capture was direct, handset speaker re-recording, screen recording or forward.
3. Record channel/codec/sampling and any call network artifacts.
4. Separate call context, claimed speaker and claimed factual message.
5. Inspect continuity, edits, overlays and noise/reverberation signatures.
6. Run locally validated audio anti-spoofing *only* if the conditions match testing population.
7. Compare corroborating records (transaction requests, official confirmations, prior authorized messages) without relying on vocal similarity alone.
8. Never use a disputed voice clip as sole authentication for payment or identity.
9. Advise independent verification through known channels if there is an ongoing fraud risk.
10. Report `SYNTHETIC SPEECH NOT ESTABLISHED` rather than “genuine person” when tests are inconclusive.

## 52. SOP D — Suspected edited screenshot or forged document

1. Identify source claim: account statement, chat message, court filing, official post or invoice.
2. Request native document or authenticated export when authorized.
3. Compare screenshot against original document and website historical UI where possible.
4. Verify signature and publication register for purported official documents.
5. Check metadata, OOXML relationships, PDF incremental updates and font/layout/graphic layers.
6. OCR text and validate dates, references, identifiers, amounts and cited legislation.
7. Trace the first appearance and repost lineage; do not over-interpret pixel filters.
8. Distinguish fabricated document from screenshot alteration and from misleading description.
9. Preserve privacy of unrelated account data.
10. Report exact altered/contradicted portions and unresolved source questions.

## 53. SOP E — Suspicious C2PA / Content Credentials claim

1. Preserve exact asset and hash.
2. Run compatible validator on native bytes in a restricted environment.
3. Record validator version, policy/trust list date, extraction flags and validation report.
4. Separate validation status from signer trust and assertion trustworthiness.
5. Inspect active manifest, ingredients, actions and AI disclosure semantics.
6. Assess whether derivation changes the content covered by signatures and bindings.
7. Confirm signer identity through relevant organizational or certificate authority channels.
8. If only a screenshot of C2PA UI exists, record it as screenshot evidence, seek original asset.
9. Compare provenance with independent first-party archive and claimed event.
10. Preserve signed original and validation outputs; present limitations explicitly.

## 54. SOP F — Suspected manipulative short-form video

1. Identify platform, post ID, source account and whether item is a duet/remix/reaction.
2. Acquire platform rendition and look for uncut original.
3. Inspect time/order of shots, caption overlays and soundtrack provenance.
4. Reconstruct original sequences from keyframe search.
5. Compare original captions with repost captions; check whether speech is dubbed or mistranslated.
6. Build timeline of publication and earliest relevant fact-checks.
7. Localize material alterations versus benign editing for presentation.
8. Corroborate key factual claims from primary sources, not the video alone.
9. Report whether deception is due to reuse, editing, captions, synthetic media or some combination.
10. Preserve specific frames/utterances used as evidence, with PTS.

## 55. SOP G — Fully synthetic or hybrid media in news context

1. Establish whether asset is labeled simulation, satirical art, game footage or illustration.
2. Identify generator/editor claims from file provenance or first-party disclosure.
3. Retrieve earlier versions, initial posting context and licensing material.
4. Determine which regions/elements may derive from real footage or stock assets.
5. Test technical clues with validated controls, not folklore “AI tells.”
6. Verify the stated event independently.
7. Separate synthetic *presentation* from false *factual implication*.
8. Mark each conclusion per segment or region with supporting evidence.
9. Avoid accusing a person or publisher of intent absent independent evidence.
10. Explain remaining uncertainty.

## 56. SOP H — Multi-camera reconstruction of a public incident

1. Identify cameras/streams by source and authorized provenance.
2. Capture native copies, clocks, orientation, aspect ratio, lens distortion and frame timing.
3. Align frames using external non-personal events and visible landmarks; document temporal offset uncertainty.
4. Compare synchronized tracks, environmental sounds and non-personal objects.
5. Verify what each camera can/cannot see due to occlusion or viewpoint.
6. Match environmental records, event times and public infrastructure chronology.
7. Detect possible edits per camera without transferring suspicion from one stream to another.
8. Create synchronized annotated derivative; keep originals untouched.
9. Require independent specialist review for any consequential physical measurement.
10. Report only public-interest time/place resolution that respects privacy.

## 57. SOP I — Public online video with suspected removed/spliced audio

1. Acquire full clip, soundtrack and original platform rendition.
2. Extract audio without transcoding if compatible; create separate PCM analysis derivative.
3. Check packet timestamps, discontinuity, dropout, channel changes and codec switches.
4. Inspect acoustic environment on both sides of disputed boundary.
5. Compare original uploads and later repost variants through waveform correlation after alignment.
6. Separate ordinary loudness compression/normalization, noise gate, subtitles, platform mixing and intentional splice.
7. Document precise sample/frame boundary with time uncertainty.
8. If no pristine reference exists, disclose that distinction.
9. Independently reproduce decisive observations.
10. Report only what the traces support.

## 58. SOP J — Photo sequence or burst alleged to be “single capture”

1. Acquire all frame files, bursts/Live Photo companions and metadata sidecars.
2. Check camera mode, burst numbering, exposure, rolling shutter and computational fusion capabilities.
3. Align frames and review moving objects and exposure deltas.
4. Compare time series with embedded image previews and original motion asset.
5. Look for panorama stitching or night-mode computational photography.
6. Distinguish legitimate in-device synthesis/fusion from misleading replacement of event content.
7. Document camera/pipeline assumptions.
8. Conclude narrowly: single sensor exposure, multi-frame camera composite, or unknown.

## 59. SOP K — Synthetic text plus counterfeit imagery in coordinated narrative

1. Break the composite claim into factual assertions, quotes and media components.
2. Identify publication network and common first sources.
3. Reverse-search imagery and verify documents; assess independent circulation.
4. Treat AI-text detector output as non-decisive.
5. Map cross-posting timestamps and editorial changes.
6. Note legitimate press-wire syndication versus coordinated deception.
7. Tie each assertion to first-party records where possible.
8. Avoid attribution of campaign intent/operator without separate evidence.
9. Produce per-claim matrix and source dependency graph.
10. Provide report with publicly verifiable URLs.

## 60. Independent peer review and quality assurance

**Peer reviewer tasks:**
- Validate evidence manifest hashes against original assets.
- Reproduce the top three technical tests from saved commands/parameters.
- Verify that no derivative was mistaken for an original.
- Check negative controls and competing hypotheses.
- Independently resolve key source citations/URLs.
- Challenge “AI probability”, C2PA trust, compressed file, metadata and archive timestamp interpretations.
- Verify anonymization, minimization and dissemination safety.
- Confirm all status labels and access limitations.
- Log disagreements and changed conclusions; preserve initial notes.

**Do not seek artificial consensus.** An unresolved disagreement can be reportable if methods differ or source artifacts cannot be reproduced.

## 61. Quality gates for high-impact cases

Require all before releasing categorical language:

| Gate | Pass criterion |
|---|---|
| G1 Claim definition | Precise, falsifiable, not ambiguous |
| G2 Original | Best available acquired; derivative limitation stated |
| G3 Integrity | Hash/custody and transformations documented |
| G4 Method | Tool versions, parameters, reference controls recorded |
| G5 Validity | Methods actually validated for relevant domain |
| G6 Independence | Corroboration sources do not merely copy same origin |
| G7 Contradictions | Alternative hypotheses/negative evidence assessed |
| G8 Peer review | Independent re-check of decisive evidence |
| G9 Legal/ethical | Privacy, consent, disclosure and authority checked |
| G10 Report | Claim-specific finding, uncertainty, cited sources and raw outputs |

If a gate fails, record it and use constrained language; do not manufacture compliance.

## 62. Common misleading arguments and corrections

| Incorrect argument | Correct reasoning |
|---|---|
| “No EXIF, therefore AI.” | Metadata routinely stripped by platforms. |
| “The hands look wrong, therefore fake.” | Visual anomaly may have many explanations; not validated proof. |
| “ELA is bright in one region, therefore Photoshop.” | Recompression residuals are content/process dependent. |
| “Detector says 99% fake.” | Score may be uncalibrated or out of domain. |
| “Five detectors agree.” | Shared training/features may make them dependent. |
| “There is no C2PA, so it is untrusted.” | C2PA adoption/retention is incomplete. |
| “C2PA says verified, event must be true.” | Signature/trust is not event-truth verification. |
| “EXIF date proves capture date.” | Device clocks and tags are editable; corroborate. |
| “Archive from Tuesday proves publication Tuesday.” | Archive date is observation date. |
| “First Google result is the source.” | Index rank does not establish earliest origin. |
| “PRNU absent means synthetic.” | Denoising/recompression/resizing may remove trace. |
| “Audio sounds robotic, so it is a clone.” | Codecs, enhancement, disability, accent, stress matter. |
| “The image is camera-original, so depicted incident happened.” | Staging, reenactment and miscaptioning remain possible. |
| “No anomalies found, therefore unedited.” | Negative result bounded by method power and asset quality. |
| “Platform URL proves owner of camera.” | Publisher account not equal creator or recording device. |
| “OCR output proves the words were there.” | OCR needs comparison to original visible pixels. |

## 63. Practical interpretation patterns

**Supports a claim:** multiple independent first-party records, original file consistency, validated test reproduces on controls and matches external chronology. State what was verified.

**Does not support a claim:** decisive contradictory first-party full recording, established earlier publication predating alleged event, demonstrable mismatch with independent event facts. Keep precise scope.

**Suggestive technical anomaly:** forensic localization result not reproduced on matched controls, inconsistent file fields with uncertain transfer pipeline. Report as lead.

**Inconclusive:** screenshot-only evidence, no native file, unavailable original, conflicting model scores, unvalidated method, archive gap or uncertain timestamps. Explicitly request the one or two high-value missing artifacts.

## 64. Tool and service selection matrix

| Starting artifact | First-line local tools | External verification | Specialist follow-up |
|---|---|---|---|
| Original JPEG/HEIC/RAW | ExifTool, `file`, ImageMagick/libvips, metadata viewer | Reverse-image search, original publisher | PRNU, Noiseprint, TruFor under validation |
| PNG screenshot | ExifTool, pixel/format inspection | UI history, official service, archived page | Layer/layout/counterfeit source analysis |
| MP4/MOV/WebM | ffprobe, MediaInfo, FFmpeg | InVID keyframes, first-party archive | GOP/PTS, video detector, cross-modal |
| WAV/MP3/Opus | ffprobe, MediaInfo, Audacity, Praat | first-party recordings when authorized | spoof benchmark, splice and codec tests |
| PDF/Office | ExifTool, qpdf, pdfinfo, ZIP inspection | official publication register | signature validation, incremental updates |
| C2PA-bearing media | c2patool + trust policy | first-party signer/original | ingredient/edit graph and external truth tests |
| URL only | HTML/HTTP capture, archive lookup | Wayback, Common Crawl, original publisher | extract/compare byte-identifiable assets |
| Social video claim | platform post preservation | search keyframes, prior versions | segment validation, dubbed audio analysis |
| Viral synthetic-image claim | reverse search and disclosures | model/publisher first party | calibrated detectors, tamper localization |

**Service privacy note:** Reverse image/audio services may receive sensitive content and metadata. When client data cannot leave a controlled environment, use local tools, public text searches, hashes or consented publication datasets instead.

## 65. Source atlas: core forensic standards, evaluation and provenance

The addresses below are **public research and tooling starting points**, not proof that each platform has been tested in your environment. Verify current releases, licenses, maintenance, API limits, processing rules and relevance before use. A source's listed capabilities are based on publicly described functions; results must be obtained and tested in the actual case.

| Resource | Purpose / evidence class | URL |
|---|---|---|
| C2PA technical specifications (v2.4) | Signed provenance data structures and validation | https://spec.c2pa.org/specifications/specifications/2.4/specs/C2PA_Specification.html |
| C2PA Content Credentials core | Content-credential architecture | https://spec.c2pa.org/specifications/specifications/2.4/specs/ContentCredentials.html |
| C2PA 2.4 implementation guidance | Binding, signing and implementation safeguards | https://spec.c2pa.org/specifications/specifications/2.4/guidance/Guidance.html |
| C2PA 2.4 crJSON | Derived JSON representation; noncanonical | https://spec.c2pa.org/specifications/specifications/2.4/crJSON/crjson-format.html |
| Content Credentials verify | Consumer-facing inspection; privacy conditions apply | https://contentcredentials.org/verify |
| `c2patool` | Read and validate available manifests via CLI | https://github.com/contentauth/c2patool |
| `c2pa-rs` | SDK integration and lower-level C2PA workflows | https://github.com/contentauth/c2pa-rs |
| NISTIR 8387 | Digital evidence preservation | https://doi.org/10.6028/NIST.IR.8387 |
| NIST OpenMFC | Media forensic evaluation and benchmarks | https://mfc.nist.gov/ |
| SWGDE image-authentication guidance | Forensic image-examination practice | https://www.swgde.org/documents/published-by-committee/imaging/ |
| SWGDE video authentication | Digital video examination | https://www.swgde.org/documents/published-complete-listing/23-v-001-best-practices-for-digital-video-authentication/ |
| SWGDE audio authentication | Digital audio examination | https://www.swgde.org/documents/published-complete-listing/15-a-001-swgde-best-practices-for-digital-audio-authentication/ |
| W3C PROV-O | Structured provenance records | https://www.w3.org/TR/prov-o/ |
| IIPC WARC specifications | Web collection/evidence archival containers | https://iipc.github.io/warc-specifications/ |
| Library of Congress Sustainability of Digital Formats | Format properties and preservation risks | https://www.loc.gov/preservation/digital/formats/ |

## 66. Source atlas: local file and metadata inspection

| Tool | Strength | Caveat / URL |
|---|---|---|
| ExifTool | EXIF, XMP, IPTC, video/container metadata | https://exiftool.org/ — tags may be wrong or stripped |
| MediaInfo | Audio/video technical/container fields | https://github.com/MediaArea/MediaInfo — not an authentication verdict |
| FFmpeg/ffprobe | Decode, remux, inspect streams, precise PTS logs | https://ffmpeg.org/ — transformations must be logged |
| ImageMagick | Format/color/derivative image processing | https://imagemagick.org/ — use isolated modern build for untrusted assets |
| libvips | Efficient imaging/derivatives | https://www.libvips.org/ — processing may alter color/metadata |
| GIMP | Manual image analysis/annotation | https://www.gimp.org/ — derivatives only |
| Krita | Image review and layer comparison | https://krita.org/ — preserve original |
| RawTherapee | RAW image inspection and controlled developing | https://www.rawtherapee.com/ — output is derived |
| darktable | RAW processing and metadata review | https://www.darktable.org/ — export not original |
| GraphicsMagick | Alternative raster image inspection | http://www.graphicsmagick.org/ — confirm security updates |
| LibRaw | Camera RAW decoding | https://www.libraw.org/ — may not cover all proprietary RAW |
| Tika | Document metadata/text extraction | https://tika.apache.org/ — untrusted file parser |
| qpdf | PDF structure and integrity checks | https://github.com/qpdf/qpdf — not signature truth |
| Poppler `pdfinfo` | PDF structural and metadata overview | https://poppler.freedesktop.org/ |
| 7-Zip | Container enumeration and protected extract | https://www.7-zip.org/ — avoid unsafe archive paths |
| `file` / libmagic | File type by magic signatures | https://www.darwinsys.com/file/ — no full-parser guarantee |

## 67. Source atlas: OSINT discovery and publication history

| Source / tool | Investigative role | URL |
|---|---|---|
| Google Lens | Public image match and visual search | https://lens.google/ |
| TinEye | Exact/near visual matches and provenance leads | https://tineye.com/ |
| Bing Visual Search | Additional image-index coverage | https://www.bing.com/visualsearch |
| Yandex Images | Alternative reverse search coverage | https://yandex.com/images/ |
| InVID-WeVerify project | Video keyframe/corroboration workflow | https://www.invid-project.eu/ |
| InVID verification plugin source | Tool architecture and feature reference | https://github.com/invideu/invid-verification-plugin |
| Internet Archive Wayback | Historical page observations | https://web.archive.org/ |
| Common Crawl | Large-scale public crawl captures | https://commoncrawl.org/ |
| Browsertrix Crawler | High-fidelity browser-based capture | https://github.com/webrecorder/browsertrix-crawler |
| ArchiveBox | Self-hosted web/media preservation | https://github.com/ArchiveBox/ArchiveBox |
| warcio | Read/write WARC | https://github.com/webrecorder/warcio |
| pywb | Replay archived web captures | https://github.com/webrecorder/pywb |
| SingleFile | Local browser page capture, subject to extension risk | https://github.com/gildas-lormeau/SingleFile |
| WACZ specification | Portable web archive packaging | https://specs.webrecorder.net/wacz/1.1.1/ |
| DocumentCloud | Publication/document analysis (service terms apply) | https://www.documentcloud.org/ |
| Wayback CDX API | URL/capture queries; API limitations apply | https://github.com/internetarchive/wayback/tree/master/wayback-cdx-server |
| Perma.cc | Legal/community archival permalinks | https://perma.cc/ |
| osintshifu catalog | Discovery of more repositories; verify original projects | https://github.com/osintshifu/awesome-osint-repos |

## 68. Source atlas: pixel forensics, manipulation localization and benchmarks

| Source | Use | URL |
|---|---|---|
| Forensically (29a.ch) | Browser image diagnostics, ELA, clone searches; **diagnostic** | https://29a.ch/photo-forensics/ |
| FotoForensics | ELA and inspection (upload/privacy limits) | https://fotoforensics.com/ |
| TruFor | Research forgery localization / reliability maps | https://github.com/grip-unina/TruFor |
| Noiseprint | Camera-model fingerprint research | https://github.com/grip-unina/noiseprint |
| DeepfakeBench | Compare deepfake detection models/data | https://github.com/SCLBD/DeepfakeBench |
| FaceForensics++ | Research manipulation benchmark | https://github.com/ondyari/FaceForensics |
| NIST OpenMFC | Controlled media forensic evaluation | https://mfc.nist.gov/ |
| Hugging Face Models | Discover model cards and checkpoints | https://huggingface.co/models |
| OpenCV | Image/video primitives, registration and optical flow | https://github.com/opencv/opencv |
| scikit-image | Reference image-processing algorithms | https://scikit-image.org/ |
| ImageHash | Exact-ish perceptual duplicate clustering | https://github.com/JohannesBuchner/imagehash |
| imagededup | Perceptual image-duplicate candidate retrieval | https://github.com/idealo/imagededup |
| Label Studio | Ground-truth annotation for calibration/validation | https://github.com/HumanSignal/label-studio |

## 69. Source atlas: audio, speech and video examination

| Tool/source | Use | URL |
|---|---|---|
| Audacity | Waveform/spectrogram and controlled audio derivatives | https://www.audacityteam.org/ |
| Praat | Speech/acoustic measurements | https://www.fon.hum.uva.nl/praat/ |
| Sonic Visualiser | Layered waveform/spectrogram annotation | https://www.sonicvisualiser.org/ |
| librosa | Local audio DSP feature extraction | https://github.com/librosa/librosa |
| pyannote.audio | Speaker diarization (not proof of real identity) | https://github.com/pyannote/pyannote-audio |
| Whisper | ASR transcription; must be human-checked | https://github.com/openai/whisper |
| whisper.cpp | Local ASR implementation | https://github.com/ggml-org/whisper.cpp |
| ASVspoof challenge | Audio spoof/deepfake research | https://www.asvspoof.org/ |
| ASVspoof5 baselines | Research baselines / evaluation protocols | https://github.com/asvspoof-challenge/asvspoof5 |
| SpeechBrain | Audio models and reference speech tasks | https://github.com/speechbrain/speechbrain |
| WebRTC VAD | Speech activity segmentation (not authenticity detector) | https://github.com/wiseman/py-webrtcvad |
| FFmpeg | Video/audio derivation and stream analysis | https://ffmpeg.org/ |
| MediaInfo | Container/codec properties | https://mediaarea.net/en/MediaInfo |
| VLC | Independent playback/seek/rendering | https://www.videolan.org/vlc/ |
| mpv | Frame stepping/playback cross-check | https://mpv.io/ |

## 70. Source atlas: documents, OCR, geospatial and event context

| Source | Role | URL |
|---|---|---|
| Tesseract | Local OCR | https://github.com/tesseract-ocr/tesseract |
| PaddleOCR | Multi-language OCR/layout | https://github.com/PaddlePaddle/PaddleOCR |
| OCRmyPDF | OCR for scanned PDFs; output is derivative | https://github.com/ocrmypdf/OCRmyPDF |
| Docling | Structured document extraction | https://github.com/docling-project/docling |
| Google Earth | Public geographic/historical imagery | https://earth.google.com/ |
| Google Street View | Dated street-level reference | https://www.google.com/streetview/ |
| OpenStreetMap | Mapping data; verify date/currency | https://www.openstreetmap.org/ |
| Mapillary | Street-level image database | https://www.mapillary.com/ |
| SunCalc | Approximate solar position and shadow testing | https://www.suncalc.org/ |
| NASA Worldview | Remote sensing and environmental event context | https://worldview.earthdata.nasa.gov/ |
| Copernicus Data Space browser | Sentinel imagery | https://browser.dataspace.copernicus.eu/ |
| USGS EarthExplorer | Satellite/aerial data retrieval | https://earthexplorer.usgs.gov/ |
| NOAA NCEI | Historical weather and climate data | https://www.ncei.noaa.gov/ |
| Meteostat | Historical weather API/data | https://meteostat.net/ |
| OGIMET | Meteorological observational archives | https://www.ogimet.com/ |
| OpenAerialMap | Community aerial imagery | https://openaerialmap.org/ |
| PeakVisor | Terrain and mountain skylines (license/coverage limits) | https://peakvisor.com/ |

## 71. Source atlas: commercial/hosted services (access-dependent)

These may be useful, but are not automatically evidence-quality. Do not transmit confidential or unconsented content merely to test them. Verify current vendor documentation, account requirements, pricing, upload retention, model/data provenance, access logs, geographical restrictions and ability to export machine-readable findings **for the exact plan offered**.

| Service or class | Potential purpose | Caveat |
|---|---|---|
| Sensity AI — https://sensity.ai/ | Hosted synthetic-media assessment | Claims/availability and methods require current verification |
| Reality Defender — https://www.realitydefender.com/ | Hosted multi-modal detection | Need domain-specific validation and privacy review |
| Hive AI — https://thehive.ai/ | Moderation/synthetic-media classifiers | Scores not forensic probabilities |
| Truepic — https://www.truepic.com/ | Capture/provenance workflows | Verify which capture/verification functions are accessible |
| Adobe Content Credentials — https://contentcredentials.org/ | Provenance interfaces | Credentials ≠ factual truth |
| Google SynthID information — https://deepmind.google/technologies/synthid/ | Proprietary generation watermark context | Public detection capability may be limited or gated |
| Commercial news/video search systems | Historical editorial content discovery | Verify licensing, original source and index coverage |
| Platform trust & safety tools | First-party source metadata | Access generally constrained to authorized workflows |

**Do not confuse** marketing pages with examined technology or independent accuracy assessments.



## 72. A reproducible local evidence-manifest script

This minimal Python 3 script recursively inventories regular files in a **working evidence directory** and writes paths, sizes and SHA-256 hashes. It does not establish legal custody, process metadata, or safely acquire remote evidence. Run it on a preserved collection, not a live mounted suspect device. Keep output *outside* the scanned directory or explicitly exclude it. Avoid symlink traversal and document filesystem specifics.

```python
#!/usr/bin/env python3
"""Write a stable, read-only CSV hash manifest for a local case directory."""
import argparse
import csv
import hashlib
import os
from pathlib import Path
from datetime import datetime, timezone

def sha256(path: Path) -> str:
    digest = hashlib.sha256()
    with path.open("rb") as f:
        for chunk in iter(lambda: f.read(1024 * 1024), b""):
            digest.update(chunk)
    return digest.hexdigest()

def main():
    ap = argparse.ArgumentParser()
    ap.add_argument("root", type=Path)
    ap.add_argument("output", type=Path)
    args = ap.parse_args()
    root = args.root.resolve(strict=True)
    output = args.output.resolve()
    if not root.is_dir():
        raise SystemExit("Input must be a directory")
    if output == root or root in output.parents:
        raise SystemExit("Output must be outside the scanned directory")
    records = []
    for base, dirs, files in os.walk(root, followlinks=False):
        dirs[:] = sorted(d for d in dirs if not (Path(base)/d).is_symlink())
        for name in sorted(files):
            p = Path(base) / name
            if p.is_symlink() or not p.is_file():
                continue
            before = p.stat()
            digest = sha256(p)
            after = p.stat()
            if (before.st_size, before.st_mtime_ns) != (after.st_size, after.st_mtime_ns):
                raise RuntimeError(f"File changed during hashing: {p}")
            records.append({
                "relative_path": p.relative_to(root).as_posix(),
                "size_bytes": before.st_size,
                "sha256": digest,
                "hash_time_utc": datetime.now(timezone.utc).isoformat()
            })
    output.parent.mkdir(parents=True, exist_ok=True)
    with output.open("w", encoding="utf-8", newline="") as f:
        writer = csv.DictWriter(f, fieldnames=[
            "relative_path", "size_bytes", "sha256", "hash_time_utc"
        ])
        writer.writeheader()
        writer.writerows(records)
    print(f"Wrote {len(records)} records: {output}")

if __name__ == "__main__":
    main()
```

Example:

```bash
python3 make_manifest.py "CASE-001/01-originals" "CASE-001/original-hashes.csv"
sha256sum "CASE-001/original-hashes.csv" > "CASE-001/original-hashes.csv.sha256"
```

**Caveats:** Symlink entries are skipped, hard links may appear more than once, sparse-file metadata is not preserved, permissions might prevent some reads, and a running process can change file content in ways not captured by a simple mtime/size check. For legally contested evidence use an approved imaging procedure and compare against source/export tool manifests.

## 73. A controlled image comparison recipe

**Only for a known pair**, not for proving an unknown “original.” First ensure both images depict the same scene and are registered to a common coordinate system. Even small resizing/color differences yield large pixel differences.

```bash
set -eu
mkdir -p derived/diff
magick "trusted_reference.png" -auto-orient \
  "derived/diff/reference-oriented.png"
magick "questioned.png" -auto-orient \
  "derived/diff/questioned-oriented.png"
# Pixel diff is meaningful only after geometric/color alignment:
compare_status=0
magick compare -metric AE \
  "derived/diff/reference-aligned.png" \
  "derived/diff/questioned-aligned.png" \
  "derived/diff/absolute-diff.png" 2> "derived/diff/AE.txt" || compare_status=$?
printf '%s\n' "$compare_status" > "derived/diff/compare.exit-status"
case "$compare_status" in
  0) printf 'Images match under the chosen comparison.\n' ;;
  1) printf 'Images differ under the chosen comparison.\n' ;;
  *) printf 'Comparison failed; inspect AE.txt before interpreting results.\n' >&2
     exit "$compare_status" ;;
esac
```

The `reference-aligned.png`/`questioned-aligned.png` are **not automatically created above**; explicitly create and document registration derivatives before the compare step. Auto-orienting may not account for mirror flips, perspective, cropping, color changes or lens distortion. “Difference pixels” are not “forged pixels.”

Use registration landmarks/feature correspondences with robust outlier rejection; visually inspect correspondences. Record transformation matrix, interpolation method and quality residuals.

## 74. A reproducible audio-segment review recipe

Convert only a **working copy** for listening, inspect the complete original and save transformation parameters. Extract with time parameters documented:

```bash
mkdir -p derived/audio-segments
# Starts at ~32.50 s, lasts 12.00 s; output is a newly encoded derivative.
ffmpeg -ss 32.50 -i "source.mp4" -t 12.00 -vn \
  -c:a pcm_s24le "derived/audio-segments/segment_32.50-44.50.wav"
```

Seeking and resampling may shift exact sample boundaries depending on codecs and options. For sample-level claims, decode the complete audio once with a documented delay/priming policy, then cut exact sample indices and retain a mapping to source PTS.

For two suspected identical passages, align at sample or spectrogram feature level **after** accounting for codec delays. High correlation may indicate re-used source audio but does not alone prove malicious editing.

## 75. Incident/media chronology template

| ID | Kind | Event in local TZ | Normalized UTC | Tolerance | Evidence | Source independence |
|---|---|---|---|---|---|---|
| T001 | Alleged capture | Unknown | Unknown | Unknown | E001 tag | Not independently verified |
| T002 | First verified published copy | Observed timestamp | Timestamp | ± uncertainty | S003 publisher | Publisher only |
| T003 | Archive capture | Crawl timestamp | Timestamp | Archive-specific | S004 archive | Independent capture of published content |
| T004 | Analyst acquisition | Exact recorded | Exact recorded | Clock calibration | E005 custody | Examiner action |

Do not fill unknown capture timestamps from upload times. Mark ambiguous date formats (`10/09/2026`) as ambiguous unless the locale is independently established.

## 76. Evidence register template

| Evidence ID | Asset/source | Original or derivative? | Hash | Collector | Date UTC | Rights/access | Stored path |
|---|---|---|---|---|---|---|---|
| E001 | [Native video] | Original acquisition | SHA256 | [Name] | [Time] | [Basis] | [Path] |
| E002 | [Frame at PTS] | Derived from E001 | SHA256 | [Name] | [Time] | Same case | [Path] |
| E003 | [Platform copy] | Distinct distribution asset | SHA256 | [Name] | [Time] | [Basis] | [Path] |

## 77. Tool execution register template

| Run ID | Source asset/hash | Tool/version | Invocation or configuration | Timestamp UTC | Exit status | Output ID/hash | Interpretation limitations |
|---|---|---|---|---|---|---|---|
| R001 | E001 / hash | ExifTool x.y | `-a -G1 -s -json` | [time] | [code] | O001/hash | Tags unverified |
| R002 | E001 / hash | ffprobe x.y | `-show_format ...` | [time] | [code] | O002/hash | Parser coverage |
| R003 | E001 / hash | c2patool x.y | [command] | [time] | [code] | O003/hash | Validator trust policy |

## 78. Source register and citation verification

Every cited source should include:
`[S###] issuer / document title / full URL / source type / original event date / publication date / last revision where known / access UTC date / content examined (full file, page, snippet, screenshot) / source reliability / information credibility / limitations / whether corroboration is independent`.

Quote minimally; trace consequential claims to primary records. Do not convert a citation on a tool README into evidence that a specific case media item was tested. State `SOURCE REVIEWED`, `TOOL NOT EXECUTED` where applicable.

## 79. Hypothesis comparison matrix

| Hypothesis | Predicted observations | Supporting observations | Disconfirming observations | Missing high-value test |
|---|---|---|---|---|
| H1: Native camera capture with no material edit | Consistent device/export, source first-party, scene corroborated | [ids] | [ids] | Native file / device |
| H2: Legitimate edited real footage | Transcoding/edit history; same event still verifiable | [ids] | [ids] | Full-length source |
| H3: Synthetic segment inserted | Localized trace, independent signed edit/disclosure, original mismatch | [ids] | [ids] | Controlled detector / source |
| H4: Old genuine footage miscapped | Earlier verified publication/context mismatch | [ids] | [ids] | Earliest source |
| H5: Staged genuine footage | Genuine acquisition, event claim independently contradicted | [ids] | [ids] | First-person verified event records |
| H6: Insufficient data | Only low-quality derivative available | [ids] | [ids] | Native evidence |

Do not force a “winner”; document how each item changes the assessment.

## 80. Structured finding syntax

For each important claim, use:

```text
FINDING ID:
Tested proposition:
Finding class: VERIFIED / SUPPORTED / INFERENCE / CONFLICT / UNRESOLVED
Evidence IDs:
Source IDs:
Method + version + parameters:
Observation (what tool/file objectively displayed):
Interpretation (narrow inference):
Alternative explanation(s):
Validation controls:
Independent corroboration:
Confidence: HIGH / MEDIUM / LOW and why
Uncertainty / gaps:
What would change the conclusion:
Reviewer status:
```

In a publication-facing report separate brief understandable explanation from technical annexes. Include a description of any alteration for privacy (blurring) applied to the **published report figure**, not the original evidence.

## 81. Reporting outcome language

Use exact, conservative claim-specific categories:

- `DEMONSTRATED DIFFERENCE`: two authenticated versions have a precisely documented difference; nature/origin may remain unknown.
- `CREDENTIALED PROVENANCE VERIFIED`: asset binding/signature/trust passed under policy P at time T; assertions remain subject to independent truth assessment.
- `ORIGINAL-SOURCE MATCH FOUND`: questioned excerpt matches authenticated source within specified transforms.
- `CONTEXT FALSE / MISATTRIBUTED`: publication history or independent context contradicts the claimed event/time/place.
- `MANIPULATION SUPPORTED`: multiple validated observations support a specific alteration; no unsupported operator attribution.
- `SYNTHETIC CONTENT SUPPORTED`: validated evidence supports synthetic region/segment with identified scope and limitations.
- `NO MATERIAL ALTERATION FOUND BY METHODS USED`: negative result with sensitivity limitations, not global “authentic.”
- `INCONCLUSIVE`: insufficient/conflicting evidence.
- `NOT TESTED`: tool/source access, legal or safety limit.

## 82. Case report skeleton

```markdown
# Digital Media Authenticity, Provenance & Forensics — Case Report

## Executive summary
- Question, strongest supported answer, confidence, key limit.

## Scope / ethics / legal authority
- Case ID, collection boundaries, private-data protections.

## Tested propositions
- Claim P1 ... Pn, falsifiable alternatives.

## Evidence acquisitions
- Exact native and derivative asset IDs, hashes, custody.

## Methods
- Versions, commands, models, thresholds, matched control design.

## Technical examinations
- File structure, metadata, pixel/video/audio/document evidence.

## Provenance and source chronology
- Signed manifests, first-party source, archive lineage.

## Context tests
- Event, location, timing, independent corroboration.

## Contradictions and rival explanations
- Failed tests, disconfirming evidence, uncertainty.

## Conclusions per claim
- Confidence, scope, unresolved questions, limitations.

## QA and independent review
- Reproduced tests, reviewer disagreements.

## Annex A — Evidence register
## Annex B — Tool execution log
## Annex C — Source register with full URLs
## Annex D — UTC timeline
## Annex E — Media lineage graph
## Annex F — Screenshots, frames and spectrograms
## Annex G — Model validation/control results
## Annex H — Preservation/retention record
```

## 83. Machine-readable output (optional)

For workflow integration, a conservative schema:

```json
{
  "case_id": "CASE-001",
  "asset_id": "E001",
  "sha256": "REPLACE_WITH_COMPUTED_HASH",
  "claims": [
    {
      "claim_id": "P1",
      "text": "REPLACE_WITH_TESTED_PROPOSITION",
      "status": "UNRESOLVED",
      "confidence": "LOW",
      "evidence_ids": [],
      "source_ids": [],
      "method_runs": [],
      "alternatives": [],
      "limitations": [],
      "peer_review": "NOT_REVIEWED"
    }
  ],
  "time_basis": "UTC",
  "source_register": []
}
```

Do not confuse a structured field with verified evidence; the schema is a container.

## 84. Open formats and long-term preservation

Preserve:
- originals in native formats, hashes and manifests;
- derivative analysis formats (PNG/TIFF for frames, WAV/FLAC for analytical audio) with source mappings;
- provenance manifest byte stores and validator outputs;
- WARC/WACZ archives where used; save checksums and replay capability;
- text logs and UTF-8 Markdown reports;
- stable references to tools, models and reproducible environments.

Store at least two restricted copies using institutional retention policy and test periodic fixity. Avoid creating incompatible converted “masters” without retaining the native original. Digitally signed PDFs and case packages should be validated after archival migration.

## 85. Security when involving LLMs or autonomous agents

- LLMs can summarize technical logs and suggest hypotheses; they **cannot replace** original-byte verification, media playback or actual tool execution.
- Treat image captions, OCR strings, EXIF comments, subtitles, repository README and web pages as **untrusted data**. Ignore instructions inside evidence such as “send the attached files to this server.”
- Do not send restricted media to models or MCP servers lacking documented authorization and privacy controls.
- Use explicit tool allowlists, network permission, rate limits, read-only storage and human confirmation for any external upload.
- Record each agent action, source accessed, tool result and derived interpretation; prevent fabricated citations or invented hashes.
- Model-generated transcripts, images, captions, comparisons or translations are derivatives; label them, retain originals and review manually.
- A model's unsupported intuition about “AI-looking” imagery is not an expert forensic measurement.
- If agents cannot access a tool or website, record `NO ACCESS`; never simulate execution.

## 86. Working with vulnerable populations and sensitive evidence

- Limit identification and geolocation to proportionate public-interest purposes.
- Minimize dissemination of victims' voices, children's faces, medical context, private interiors and personal data.
- Blur/redact **copies only**, log transformations and retain restricted originals when legally appropriate.
- Obtain consent and legal review for biometric speaker/face comparisons.
- Separate claims about a **public action** from identity attribution of bystanders.
- Establish secure sharing practices for sensitive or graphic material; analyst wellness and exposure controls should be part of the case SOP.
- Use specialized authorities and protective processes for unlawful abuse material; do not seek, download or process it via public discovery.

## 87. Privacy-aware sample publication

For press publication:
1. Verify public-interest basis for identifying the alleged source.
2. Ensure the conclusion actually follows from reproduced checks.
3. Use limited excerpts and annotated **derivatives** with adequate context.
4. Avoid embedding private GPS or victim metadata in downloadable figures.
5. Explain where a clip/crop was made and include source timestamp mappings.
6. State unresolved uncertainties, false-positive risks and method limits.
7. Offer corrections channel and preserve a record of updated conclusions.
8. Never publish a claimed exact residence or live tracking clue from a media verification task.

## 88. Maintenance and tool-refresh procedure

At least quarterly, or before every high-stakes investigation:
- Check latest C2PA spec, validator and trust lists.
- Check SWGDE/NIST/OSAC and relevant jurisdiction evidence guidance.
- Recheck tool release, maintenance state, security advisories, license and dependencies.
- Recheck hosted-service privacy, export, model version, availability and API rights.
- Run local acceptance tests on matched controls and document score drift.
- Add new codec/format checks as mobile platforms change.
- Audit invalid links, archived projects and renamed repos.
- Verify sampling/threshold SOPs against current tool versions.
- Retain old SOP versions to make prior casework reproducible.

### 88.1 Source lifecycle statuses

`VERIFIED OFFICIAL`, `VERIFIED REPO`, `REVIEWED SECONDARY`, `ACCESS-RESTRICTED`, `RESEARCH / VALIDATION REQUIRED`, `ARCHIVED / HISTORICAL`, `UNAVAILABLE`, `NOT CHECKED`. A link being publicly reachable is not evidence the tool works, is safe or is suitable for the case.

## 89. Field checklists by decision stage

### Intake and acquisition

- [ ] Scope and consent/legal basis documented.
- [ ] Hypotheses and event claims separated.
- [ ] Source URLs/post IDs and source context captured.
- [ ] Highest-quality available original acquired or limitation stated.
- [ ] Asset hashes computed and originals protected.
- [ ] Derived artifacts have parent links and transformation logs.
- [ ] Time zones and event vs publication timestamps separated.
- [ ] Sensitive content and upload restrictions reviewed.

### Image

- [ ] True file format and metadata scopes inspected.
- [ ] Original/publisher source searched.
- [ ] Independent reverse search and crop/OCR checks performed.
- [ ] Compression and camera assumptions documented.
- [ ] Suspicious region tests have matched controls.
- [ ] AI-model scores calibrated or recorded as non-dispositive.
- [ ] Scene context independently examined.

### Video

- [ ] Container/streams, FPS/VFR, PTS and timebase inspected.
- [ ] High-information keyframes extracted with mapping.
- [ ] Continuity/cut/reorder hypotheses tested.
- [ ] Audio/video alignment assessed.
- [ ] Compression, filters and platform transformations accounted for.
- [ ] Disputed segments have exact time intervals and derivation links.

### Audio

- [ ] Native recording and codec chain preserved.
- [ ] Spectrogram/waveform reviewed across disputed boundaries.
- [ ] Voice identity distinguished from speech synthesis and factual truth.
- [ ] Telephony/enhancement/re-recording confounders considered.
- [ ] Transcription manually checked and uncertainty marked.
- [ ] Anti-spoof model operating conditions validated or withheld.

### Provenance and context

- [ ] C2PA presence/binding/signature/trust/assertions distinguished.
- [ ] crJSON not treated as independently verified manifest.
- [ ] Published claims traced to first-party originals.
- [ ] Archive capture dates separated from event dates.
- [ ] Geolocation/chronolocation limited to necessary precision.
- [ ] Source dependencies and conflicting evidence documented.

### Reporting

- [ ] Findings distinguish observation and inference.
- [ ] Every consequential statement cites evidence/source IDs.
- [ ] Model outputs are not expressed as invented event probabilities.
- [ ] “No findings” not equated to “not altered.”
- [ ] Peer reviewer reproduces decisive checks or limitation stated.
- [ ] Case evidence and public derivatives stored separately.
- [ ] Retention, corrections and dissemination approved.

## 90. Practical training and tabletop exercises

Use licensed or self-created safe data with ground truth.

| Exercise | Challenge | Expected trainee deliverable |
|---|---|---|
| A | JPEG recompressed five times without malicious edit | Why ELA does not prove manipulation |
| B | Screenshot of a genuine article with misleading caption | Provenance/caption separation |
| C | Real photo with benign AI denoise | Distinguish AI processing from generated event |
| D | Synthetic image with no anatomical errors | Source-based reasoning vs folklore |
| E | Authenticated C2PA image of a staged scene | Signature versus event-truth explanation |
| F | Valid signed edit plus AI-generated insert | Ingredient/action graph and region claim |
| G | VFR camera video with dropped packet | False temporal anomaly assessment |
| H | Old disaster video reposted as current | Earliest-source and event chronology |
| I | Voice message with aggressive denoise | Anti-spoof confounders |
| J | Genuine audio spliced at two words | Sample-level localization and source comparison |
| K | PDF incrementally saved after legitimate signature | Correct signed-byte scope and update validation |
| L | Multiple outlets quoting same false initial source | Source dependence, no circular confirmation |

Scoring should reward correct uncertainty and reproducibility, not simply detecting more fakes.

## 91. Final review checklist for this guide

- Revalidate all external URLs and exact product versions before operational use.
- Treat open-source repositories as candidate tools requiring security review.
- Treat hosted platforms as potentially privacy-sensitive and access-dependent.
- Keep this document and derived commands version-controlled.
- Report observed evidence, not what a tool is generally capable of.
- Never invent first-seen dates, EXIF, C2PA manifests, hashes, geolocation, identity, model accuracy or court admissibility.
- Use qualified experts for dispositive contested examinations and local evidentiary standards.
- Prefer high-quality, testable *findings* over large counts of unrelated “AI red flags.”

## 92. Source review notes and provenance

The following **primary and original-project** sources informed this guide's methodology. This is not a claim that all software listed in the tool atlas was installed, executed or laboratory-tested. Tool catalogs are discovery points, and technical claims should be rechecked at the original project/documentation release when used in a live case.

| ID | Authority/source | Scope | Full official URL |
|---|---|---|---|
| S001 | Coalition for Content Provenance and Authenticity | Technical specification v2.4, April 2026 | https://spec.c2pa.org/specifications/specifications/2.4/specs/C2PA_Specification.html |
| S002 | C2PA | Content Credentials / trust semantics | https://spec.c2pa.org/specifications/specifications/2.4/specs/ContentCredentials.html |
| S003 | C2PA | Implementation guidance / binding | https://spec.c2pa.org/specifications/specifications/2.4/guidance/Guidance.html |
| S004 | C2PA | Derived crJSON format | https://spec.c2pa.org/specifications/specifications/2.4/crJSON/crjson-format.html |
| S005 | NIST | Digital Evidence Preservation, NISTIR 8387 | https://doi.org/10.6028/NIST.IR.8387 |
| S006 | SWGDE | Current image-authentication and forensic image guidelines index | https://www.swgde.org/documents/published-by-committee/imaging/ |
| S007 | SWGDE | Video authentication guidance | https://www.swgde.org/documents/published-complete-listing/23-v-001-best-practices-for-digital-video-authentication/ |
| S008 | SWGDE | Audio authentication guidance | https://www.swgde.org/documents/published-complete-listing/15-a-001-swgde-best-practices-for-digital-audio-authentication/ |
| S009 | NIST | Open Media Forensics Challenge | https://www.nist.gov/publications/nist-open-media-forensics-challenge-openmfc-briefing-iird |
| S010 | Content Authenticity Initiative | `c2patool` official source | https://github.com/contentauth/c2patool |
| S011 | FFmpeg | `ffprobe` documentation | https://ffmpeg.org/ffprobe.html |
| S012 | MediaArea | MediaInfo original repository | https://github.com/MediaArea/MediaInfo |
| S013 | GRIP-UNINA | TruFor research implementation | https://github.com/grip-unina/TruFor |
| S014 | GRIP-UNINA | Noiseprint implementation | https://github.com/grip-unina/noiseprint |
| S015 | SCLBD | DeepfakeBench benchmarks | https://github.com/SCLBD/DeepfakeBench |
| S016 | ASVspoof | Research challenge and benchmarks | https://www.asvspoof.org/ |
| S017 | ASVspoof challenge maintainers | ASVspoof5 reference baselines | https://github.com/asvspoof-challenge/asvspoof5 |
| S018 | W3C | Provenance Ontology (PROV-O) | https://www.w3.org/TR/prov-o/ |
| S019 | IIPC | WARC format specifications | https://iipc.github.io/warc-specifications/ |
| S020 | Webrecorder | Browsertrix crawler repository | https://github.com/webrecorder/browsertrix-crawler |
| S021 | ArchiveBox maintainers | Archiving toolkit | https://github.com/ArchiveBox/ArchiveBox |
| S022 | ExifTool | Original project | https://exiftool.org/ |
| S023 | osintshifu | FOSS discovery catalogue | https://github.com/osintshifu/awesome-osint-repos |
| S024 | Original OSINT Tradecraft repository | Earlier AI media manual for migration comparison (historical version) | https://github.com/osintshifu/osint-tradecraft/blob/26de65e97eea94b0febfe92a3fc5414708242481/manuals/ai-media-forensics-manual.md |

**Methodological maintenance notice:** Standards, tools, trust lists, hosting policies and detector performance evolve. Recheck authoritative sources at the time of each case. This guide intentionally avoids asserting that any single algorithm, vendor or model can determine media truth with certainty.
