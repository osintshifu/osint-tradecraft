# ✅ AI Detection Checklist

![Version](https://img.shields.io/badge/version-v1.0.0-blue)  
![Last Update](https://img.shields.io/badge/updated-2026--10--09-red)

A practical checklist for examining potentially generated or manipulated images, video, audio and text. Use observations as leads for a specific claim, then test processing history, source context and alternative explanations.

No individual visual anomaly, missing metadata or detector score establishes synthetic origin. Compression, editing, camera processing and ordinary recording conditions can produce similar signals. For acquisition procedures, controls and reporting, use the [Digital Media Authenticity, Provenance & Forensics - Advanced Field Guide](../field-guides/digital-media-authenticity-provenance-field-guide.md).

## 🖼️ Image & Visual Content Verification

-  **Anatomy & Object Integrity**
    
    - Inspect hands: count fingers, check proportions, examine nail shape and placement.
        
    - Examine eyes: look for mismatched irises, unnatural reflections, symmetry that is “too perfect.”
        
    - Inspect teeth: check if rendered as a uniform block, misaligned gum lines, or blurry interiors.
        
    - Inspect ears and earrings: check for asymmetry, distortions, or blending into hair/skin.
        
    - Check accessories (glasses, hats, jewelry) for warped edges, melting, or blending artifacts.
        
-  **Clothing & Fabrics**
    
    - Look for stitching errors, inconsistent textures, or repeating patterns.
        
    - Inspect logos and printed text on clothing; blur or distorted letters can also result from resolution, motion or compression.
        
    - Check folds and shadows in fabric for natural consistency.
        
-  **Background Consistency**
    
    - Inspect signage and text in the background for legibility.
        
    - Identify warped objects (lamp posts, buildings, cars).
        
    - Check perspective lines: ensure vanishing points are consistent.
        
-  **Lighting & Shadows**
    
    - Test shadows against plausible light sources, including multiple lamps, flash, reflections and compositing; do not assume a single source.
        
    - Validate intensity and direction of light on different objects.
        
    - Use [SunCalc](https://www.suncalc.org/) to test a claimed location and time against solar geometry, allowing for measurement uncertainty.
        
-  **Reflections**
    
    - Inspect mirrors, windows, and water surfaces.
        
    - Ensure reflected objects match reality (orientation, size, color).
        
-  **Technical Checks**
    
    - Run **reverse image search** on full image and cropped anomalies.
        
    - Use **Error Level Analysis (ELA)** via [Forensically](https://29a.ch/photo-forensics/) on suitable JPEGs with matched processing controls. Bright regions alone do not prove manipulation.
        
    - Inspect for cloning or copy-paste elements.
        
    - Review **EXIF metadata** using [ExifTool](https://exiftool.org/).
        
    - Validate GPS and timestamps against claimed context.
        

## 🎥 Video Verification

-  **Frame-by-Frame Analysis**
    
    - Scrub video frame by frame for inconsistencies.
        
    - Check lips vs. phonemes for sync accuracy.
        
    - Look for flickering artifacts or blending errors.
        
-  **Motion & Blur**
    
    - Inspect motion blur and sharp edges, accounting for shutter speed, stabilization, frame interpolation and transcoding.
        
    - Look for “halo” effects or ghosting in moving objects.
        
-  **Context Checks**
    
    - Verify landmarks, signs, and clothing seasonality.
        
    - Cross-check weather with [Meteostat](https://meteostat.net/) or [OGIMET](https://www.ogimet.com/).
        
    - Use [SunCalc](https://www.suncalc.org/) for shadow analysis.
        
-  **Technical Tools**
    
    - Extract thumbnails and keyframes with [InVID](https://www.invid-project.eu/tools-and-services/invid-verification-plugin/).
        
    - Run reverse video searches.
        
    - Analyze encoding for unusual compression signatures.
        
-  **AI Detection**
    
    - If authorized to upload, use [SensityAI](https://sensity.ai/) or another suitable detector as a supporting test. Record model/version, input processing, controls and known limitations.
        
    - Use a validated model suited to the tested manipulation and media conditions. [FaceForensics++](https://github.com/ondyari/FaceForensics) is a research dataset and benchmark, not a standalone authenticity verdict.
        

## 🔊 Audio Verification

-  **Listening Checks**
    
    - Identify robotic cadence, flat intonation, or overly clean delivery.
        
    - Check for missing human sounds (breathing, mouth clicks, filler words).
        
    - Detect looping or repetitive background noise.
        
-  **Spectrogram Analysis**
    
    - Generate spectrograms in [Audacity](https://www.audacityteam.org/) or [Praat](https://www.fon.hum.uva.nl/praat/).
        
    - Look for:
        
        - Clean unnatural high frequencies.
            
        - Banding artifacts.
            
        - Missing natural harmonics.
            
-  **Environmental Verification**
    
    - Validate background sounds (birds, traffic, wind) against claimed setting.
        
    - Compare ambient audio with expected acoustics (e.g., indoor echo vs. outdoor open field).
        
-  **Technical Tools**
    
    - Test suspected synthetic speech with a validated audio anti-spoofing model and matched authentic/synthetic controls. [ASVspoof](https://www.asvspoof.org/) provides research benchmarks; benchmark performance does not establish case-specific accuracy.
        
    - Compare recording conditions and speech characteristics with authorized reference samples; voice similarity alone does not establish speaker identity or exclude cloning.
        
    - Analyze jitter/shimmer metrics in Praat only where the recording and method support them; these measurements are not a general synthetic-voice test.
        

## 📝 Textual Verification

-  **Linguistic Checks**
    
    - Identify repetitive scaffolding (e.g., “In conclusion, …”).
        
    - Look for vague or generic phrasing without specifics.
        
    - Check for fabricated citations, URLs, or ISBNs.
        
-  **Factual Validation**
    
    - Spot-check quotes and references against primary sources.
        
    - Cross-verify dates, events, and names in OSINT databases.
        
-  **Technical Tools**
    
    - Treat [GLTR](http://gltr.io/) or [DetectGPT](https://github.com/eric-mitchell/detect-gpt) as research methods with model, language and sampling assumptions. Their scores do not prove authorship.
        
    - Perform stylometric comparison with JStylo.
        
    - If testing a text detector, validate it against matched human and generated samples. Correlated model outputs are not independent corroboration; do not report a score as an AI-authorship probability.
        

## 🌍 Contextual & Environmental Consistency

-  Validate location using Google Earth and Street View.
    
-  Cross-check building architecture with regional styles.
    
-  Verify vegetation/season (trees in bloom vs. claimed season).
    
-  Validate weather data with [Meteostat](https://meteostat.net/) or [OGIMET](https://www.ogimet.com/).
    
-  Check holidays, political events, or known gatherings on claimed date.
    
-  Match crowd size against known venue capacity.
    
## 📊 Metadata & Technical Fingerprints

-  **EXIF Analysis**
    
    - Extract with [ExifTool](https://exiftool.org/).
        
    - Investigate improbable fields against acquisition and processing history. Missing metadata is common and does not establish manipulation.
        
    - Detect editing software tags (Stable Diffusion, MidJourney, Photoshop).
        
-  **Compression & Encoding**
    
    - Validate JPEG quantization tables.
        
    - Compare video codecs against known device profiles.
        
-  **Sensor Noise, PRNU & Camera-Model Traces**
    
    - Use [Noiseprint](https://github.com/grip-unina/noiseprint) for camera-model traces and potential localization, subject to validation. It does not identify an individual physical sensor.
        
    - For individual-camera attribution using PRNU, use an appropriate validated method, adequate reference images and controls for compression, resizing and processing.
        
-  **Provenance Checks**
    
    - Check for C2PA manifests on the exact rendition; distinguish signature validation, asset binding, signer trust and the assertions made.
        
    - Inspect Content Credentials validation results and edit history. A valid credential does not prove that a depicted event occurred; an absent credential does not prove fabrication.
        
    - Run Google SynthID watermark checks if available.
        
## 🤝 Peer Review & Validation

-  Share findings with a second analyst for independent validation.
    
-  Compare across multiple tools and detection methods.
    
-  Store SHA-256 hashes of original files and verify them after transfers. Record MD5 only if a legacy workflow requires it, alongside SHA-256.
    
-  Maintain chain of custody logs for evidentiary purposes.
    
-  Document all anomalies with annotated screenshots.
    
-  Record all commands, queries, and tools used for auditability.
    
## 🛠️ Quick Access Tools

|Tool|Type|Purpose|
|---|---|---|
|[Forensically](https://29a.ch/photo-forensics/)|Image forensics|Error level analysis, clone detection, metadata review|
|[InVID Plugin](https://www.invid-project.eu/tools-and-services/invid-verification-plugin/)|Video verification|Extract thumbnails, reverse video search, metadata analysis|
|[ExifTool](https://exiftool.org/)|Metadata extraction|Inspect and validate EXIF and file metadata|
|[GLTR](http://gltr.io/)|Text research|Inspect token statistics under a selected language model; not proof of authorship|
|[DetectGPT](https://github.com/eric-mitchell/detect-gpt)|Text research|Research method for generation detection under stated model assumptions|
|[Noiseprint](https://github.com/grip-unina/noiseprint)|Image forensics|Camera-model traces and manipulation localization; not individual-sensor attribution|
|[Audacity](https://www.audacityteam.org/)|Audio analysis|Waveform and spectrogram inspection|
|[Praat](https://www.fon.hum.uva.nl/praat/)|Audio forensics|Acoustic analysis of speech and voice patterns|
|[Meteostat](https://meteostat.net/)|Contextual data|Historical weather validation|
|[SunCalc](https://www.suncalc.org/)|Contextual analysis|Validate shadows and sun positions by time and place|
|[SensityAI](https://sensity.ai/)|AI detection|Deepfake and synthetic media detection services|
