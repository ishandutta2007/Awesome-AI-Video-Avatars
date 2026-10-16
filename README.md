# Awesome-AI-Video-Avatars

# Top AI Video Avatars Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Talking-Head Synthesis, Real-Time Face Swap & VTuber Automation*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **AI Video Avatars**. These tools enable creators and developers to generate talking-head videos from a single photo, swap faces in real time for live streaming, and build VTuber avatars that lip-sync to microphone input—without expensive rendering infrastructure.

**Examples** include Synthesia, HeyGen, D-ID, Runway, Pika, Elai.io, Colossyan, DeepBrain AI, Hour One, and Rephrase.ai (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, real-time face swap, and open talking-head generation—ideal for content creators, streamers, and developers seeking transparent, vendor-independent avatar infrastructure.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Synthesia](https://www.synthesia.io/)**  
  AI avatar video platform with 230+ avatars and 140+ languages. Features **custom avatar creation**, **voice cloning**, and **one-click video generation** from text. **The enterprise standard for L&D and corporate communications.**

- **[HeyGen](https://www.heygen.com/)**  
  AI avatar and voice cloning platform with **video translation**, **personalized video at scale**, and **interactive avatars**. Features **Avatar IV** for expressive talking heads.

- **[D-ID](https://www.d-id.com/)**  
  Photo-to-talking-avatar platform with **Creative Reality Studio**. Animates still photos with speech for marketing, training, and customer service. **Freemium tier available.**

- **[Runway](https://runwayml.com/)**  
  AI video generation and editing platform with **Gen-3/Gen-4** video models. Features **Act-One** for performance capture and **motion brush** for animated regions.

- **[Pika](https://pika.art/)**  
  AI video generation with **Pikaffects** for creative transformations. Features **Pika Labs** for text-to-video and image-to-video.

- **[Elai.io](https://elai.io/)**  
  AI video generation with avatars, voiceovers, and templates. Features **custom avatar creation** and **PowerPoint-to-video** conversion.

- **[Colossyan](https://www.colossyan.com/)**  
  AI video platform for workplace learning with **avatars, voice cloning, and translation**. Features **interactive video** and **SCORM export**.

- **[DeepBrain AI](https://www.deepbrain.io/)**  
  AI human video synthesis with **realistic avatars** and **multi-language support**. Features **AI Studios** for text-to-video and **AI Kiosk** for interactive avatars.

- **[Hour One](https://hourone.ai/)**  
  AI video platform with **presenter avatars** and **text-to-video generation**. Features **custom avatar creation** and **brand templates**.

- **[Rephrase.ai](https://www.rephrase.ai/)**  
  AI-generated video platform with **digital avatars** and **personalized video at scale**. Acquired by Adobe (2022).

## Open-Source GitHub Projects

- **[LongCat-Video-Avatar 1.5 (Meituan)](https://github.com/meituan-longcat/LongCat-Video-Avatar)**  
  **Commercial-grade digital human video generation model** (MIT) — **the first open-source avatar model to comprehensively outperform HeyGen in blind benchmarks** . **User Preference Win Rate**: **65.9% vs Kling Avatar 2.0**, **61.1% vs OmniHuman-1.5**, **54.3% vs HeyGen** . **Three core upgrades**: **Whisper-large audio encoder** (replacing Wav2Vec2) for more accurate lip movements on long sentences, fast speech, and singing; **multi-stage data augmentation** with multi-person conversation, silent, and emotional data for open-domain generalization; **GRPO human preference alignment** for hand generation in e-commerce/livestream scenarios . **15x faster inference** via Distributed Matching Distillation (50 steps → 8 steps) and single shared base model + LoRA adapters—**10-second video in ~1 minute** . **Runs on a single NVIDIA H200 (80GB VRAM)** . **Supports** real people, anime, animals, multi-person conversations, and singing .

- **[Deep-Live-Cam](https://github.com/hacksider/Deep-Live-Cam)**  
  **Real-time face swap and one-click video deepfake with a single image** (open-source, **96,916 GitHub stars**) . **The most widely adopted open-source face swap tool** . **Three-click workflow**: select face → select camera → press live . **Features**: Mouth Mask (retain original mouth for accurate movement), Face Mapping (different faces on multiple subjects simultaneously), **OBS virtual camera support** for streaming . **Model engines**: Inswapper (128x128), HyperSwap (256x256, **200% improvement**), ReSwapper, Decart Live (cloud real-time diffusion), FLUX Live (real-time prompt-based face editing at 30fps, requires RTX 5090/6000) . **Pre-built binaries** for Windows (DirectML, CUDA, OpenVINO), macOS (CoreML), and Linux . **Note**: Model used is **non-commercial only** .

- **[FreeVideoAI](https://github.com/333kjp/freevideoai)**  
  **Free open-source digital human video studio** — one script → one talking-head video with your own face and voice . **Three engine tiers auto-detected by GPU**: **Cloud tier** (no GPU required, OmniHuman cloud engine, ¥1/sec), **Standard tier** (4-16GB VRAM, VoxCPM voice cloning + MuseTalk lip sync, ~8 min for 1-minute video, free), **Flagship tier** (16GB+ VRAM, + LatentSync 1.6 / EchoMimic V3 local, 1-10 min, free) . **Features**: zero-shot voice cloning (5-20 seconds of clean audio), **auto B-roll mixing** with LLM-planned insertion points and Seedance 2.0 product/scene generation, **multi-shot virtual camera** (close-up/medium shot alternation), **production room** with 9-stage visualization, word-level karaoke subtitles, BGM, filters/transitions, cover/title auto-generation, and multi-platform publishing checklist . **Engineering**: SQLite state machine for resumable runs, TTS result caching, per-stage GPU exclusivity, degradation chain logging .

- **[Enliven](https://github.com/CoCoNuT-sTuDiOs/Enliven)**  
  **AI avatar animation with real expression transfer** (MIT/Apache-2.0) — **commercial-safe** with no research restrictions . **Three inputs**: static avatar photo + driving video (real person with expressions) + optional audio . **Output**: animated avatar video where the avatar mimics the real person's expressions, head movements, and blinks . **Key innovation**: **Real expression transfer from actual driving video**, not audio-guessed—full 3D head rotation, nods, and tilts . **Pipeline**: LivePortrait (expression & pose transfer via MediaPipe Face Mesh, commercial-safe) + optional GFPGAN face enhancement . **Requirements**: Python 3.10+, 8GB RAM minimum (16GB+ recommended), GPU recommended (CPU-only takes 13-20+ hours per 10-second video) .

- **[higgsfree](https://github.com/kunal12203/higgsfree)**  
  **Open-source AI talking-avatar video generation pipeline** — consent video + script → photorealistic talking-head video with **face identity preserved, voice cloned, and lips synced** . **Modular, self-hostable** with reusable building blocks: **PuLID SDXL + RealVisXL** for face identity preservation, **Chatterbox TTS** for zero-shot voice cloning, **Sonic (CVPR 2025)** for audio-driven mouth animation, and scene compositing (studio, cafe, desk) . **Three pipelines**: `avatar_studio` (20GB VRAM, full scene), `portrait` (16GB, head-only), `text_to_video` (24GB, CogVideoX-5b) . **Every PR run automatically on real GPU and scored for quality** before merge . **Docker support** with stage caching for resumable runs .

- **[AVTR-1 (Avaturn Live)](https://github.com/avaturn-live/avtr-1)**  
  **Open-source real-time avatar model** — given a portrait image and dual-stream audio (speech + listening track), renders **lip-synced speech and active listening at 25 fps on a single GPU** . **Performance**: **L40 (84ms/chunk, 2.4× real-time)**, **A100 (91ms, 2.2×)**, **RTX 4060 Ti (166ms, 1.2×)**, **RTX 3070 (181ms, 1.1×)** . **Requires**: CUDA 12.x, TensorRT 10.x, Ampere+ GPU . **License**: AVTR-1 Community License with explicit prohibitions on **non-consensual deepfakes, impersonation, harassment, exploitation of minors, automated decisions affecting legal rights, and military/weapons applications** . **Designed for 25 fps output at near-frontal portrait input**—out-of-distribution poses degrade quality . **Trained on publicly available video content**—may perform unevenly across underrepresented demographics .

- **[facestream](https://github.com/philipp-eisen/facestream)**  
  **Web app for real-time face swap without a powerful machine** (open-source) . **Uses Deep-Live-Cam model** but runs on **remote server via WebRTC**—solves the M1 Mac 0.5 FPS problem . **Deployable on Modal** (serverless GPU platform) with `uv run modal deploy` . **TURN server support for cellular networks** via Cloudflare . **Credits**: Inspired by Deep-Live-Cam; model is **non-commercial use only** .

- **[OpenVT](https://github.com/erodozer/open-vt)**  
  **Open-source 2D VTuber software** — native Linux support, community-driven development, transparent window for OBS alpha capture, adjustable filtering for pixel art models . **VTube Studio compatible**—assets can be shared between both without adjustment . **Built in Godot** (not Unity) with entirely open-source solutions . **Supported trackers**: OpenSeeFace (separate executable), VTube Studio (TCP over Wi-Fi) . **Feature parity with VTS is a goal**, excluding complex features like plugin compatibility and VNet .

- **[Avatar Studio (JagTheHero)](https://github.com/JagTheHero/VTuberAvatarStudio)**  
  **Lightweight VTuber avatar system** — "one picture in, a live, lip-synced VTuber out" (MIT) . **Runs in browser**—no GPU required, renders in OBS browser source . **How it works**: base loops (mouth-neutral) ⊕ viseme mouth sprites = final frame . **Five-step workflow**: Design (generate portraits, upload art, or import VRM) → Animate (chained idle clips per emotion) → Mouths (viseme sprite set in character's style) → Build (mouth tracking, chroma key, sprite alignment → portable bundle) → Go Live (runtime picks mouth shape per audio frame via MFCC viseme classification + energy-driven openness) . **VRM path is fully AI-free**—portraits, expressions, and mouth sets rendered from model's own blendshapes . **Third-party**: MediaPipe Tasks (Apache-2.0) for camera-driven emotion tracking, three.js and @pixiv/three-vrm (MIT) for VRM rendering .

- **[KuroBlob AI](https://github.com/eykicuihb/KuroBlob-AI)**  
  **Web-native procedural avatar engine** (open-source) — "Living 3D Procedural Jelly Avatar Engine" . **60+ procedural emotions** with Blink-Masked Shape Morphing (0.18s blink animation for transitions) . **Animation Timeline & Montage Story Sequencer**—chain emotions, adjust durations (0.4s-6.0s), automated loop playback . **Native MP4 export** (H.264) for social media without external transcoding . **Web VTuber Mode** at 60 FPS with camera head roll/yaw tracking and 3D spherical head-eye parallax coupling . **BYOK LLM integration** (Ollama, OpenAI-compatible) with SSE streaming and real-time `[EMOTION:XYZ]` dynamic mood tagging . **AI Expression Creator Studio**—natural language prompts compile to Canvas 2D vector drawing code . **OBS Chroma Green Screen Mode** .

- **[claude-codes-influencers](https://github.com/kevinbadi/claude-codes-influencers)**  
  **Build a talking mascot that turns any script into a lip-synced vertical video** (open-source) . **Outputs 1080x1920 MP4 ready for Reels, TikTok, and Shorts** . **How it works**: your picture → Claude finds the face → mascot folder (mascot.py + sprites/) → script → voice (say/ElevenLabs/Voicebox/mic) → lip sync (Rhubarb: sounds → 9 mouth shapes) + word timings (Whisper) → animator stacks [ears/tail] + [pose] + [eyes] + [mouth] + captions → mp4 . **Three ways to create a mascot**: **Fastest** (upload picture, Claude rigs it in 2 minutes—cuts out character, finds mouth/eyes/skin/outline, renders talking mouths and blinks, checks its own work up to 3 rounds), **Best quality** (Claude Code draws from references using `draw-mascot` skill), or **hand-made** . **Needs**: Python 3.10+, ffmpeg, `ANTHROPIC_API_KEY` .

### Additional Strong Open-Source Options

- **[DeepFaceLive (iperov)](https://github.com/iperov/DeepFaceLive)** — Real-time face swap for PC streaming or video calls (31,007 GitHub stars) . **The most established alternative to Deep-Live-Cam** .
- **[VTuberAvatarStudio](https://github.com/JagTheHero/VTuberAvatarStudio)** — See Avatar Studio above.
- **[Brioche Puppet](https://store.steampowered.com/app/4286130/Brioche_Puppet/)** — Free open-source VTuber software (Steam) . MMD and VRM animation & model, MediaPipe video detector, VMC protocol motion receiver, Bullet Physics, PBR rendering, toon shading, and global illumination . **Note**: Voxel Cone Tracing GI recommended only for high-end hardware .
- **[liveportrait-joyvasa](https://pkg.go.dev/github.com/plexusone/omniavatar-core/providers/liveportrait-joyvasa)** — Local audio-driven talking-head generation on Apple Silicon MPS (MIT) . **Combines LivePortrait (MIT) and JoyVASA (MIT)** —both fully free with no revenue cap . **Uses MediaPipe (Apache-2.0) as commercial-clean replacement for InsightFace buffalo_l** (which is non-commercial) . **Performance**: ~5 min for 13.7s output on M-series, ~4GB memory .
- **[Backblaze AI Avatar Video Generator](https://github.com/backblaze-b2-samples/ai-avatar-video-generator)** — Open-source AI avatar video generator (Next.js + FastAPI + Backblaze B2) . **Script + avatar → talking-head video with synced voice** . **Pluggable providers**: D-ID (default, free trial), FAL, HeyGen documented . **Full-bucket File Explorer and generic Upload** with B2-backed scaffolding .
- Community **n8n** workflows for avatar video generation pipeline automation and social media publishing.

**Frameworks for building custom systems**: Combine **LongCat-Video-Avatar 1.5** for commercial-grade talking-head generation with **Deep-Live-Cam** for real-time face swap, **FreeVideoAI** for local voice cloning and lip sync, **AVTR-1** for real-time streaming avatars, and **Avatar Studio** or **KuroBlob AI** for VTuber automation—creating a fully self-hosted, enterprise-grade AI video avatar platform.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- **AI video avatars and face swap tools must comply with consent requirements, right of publicity laws, and data protection regulations (GDPR, CCPA, etc.).** **Never generate likenesses of identifiable individuals without explicit, informed consent.** Deep-Live-Cam's model is **non-commercial use only** .
- **Open-source video avatars have reached commercial parity.** LongCat-Video-Avatar 1.5 **outperformed HeyGen in blind benchmarks** (54.3% user preference win rate) and runs on a single H200 at **15x faster inference** (10-second video in ~1 minute) . **This is a genuine open-source alternative to commercial platforms** .
- **Real-time face swap is accessible but legally constrained.** Deep-Live-Cam has **96,916 GitHub stars** and supports **OBS virtual camera** for streaming . **The model is non-commercial only**—commercial use requires separate licensing .
- **AVTR-1's license sets the standard for responsible AI.** The AVTR-1 Community License **explicitly prohibits non-consensual deepfakes, impersonation, harassment, exploitation of minors, automated decisions affecting legal rights, and military/weapons applications** . **Deployers are responsible for confirming consent** .
- **VTuber tools are maturing rapidly.** OpenVT provides **native Linux support** and **VTube Studio asset compatibility** . Avatar Studio runs **entirely in browser with no GPU required**—renders in OBS browser source . KuroBlob AI adds **60+ procedural emotions and native MP4 export** .
- Self-hosted open-source solutions require proper GPU provisioning (16-24GB VRAM for high-quality pipelines), model management, and ongoing maintenance. **Generated content may require disclosure as AI-generated** to comply with emerging regulations (EU AI Act Article 50).
