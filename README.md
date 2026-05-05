# Awesome Video Generation [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com) [![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

A curated list of AI video generation APIs, SDKs, and production-ready tools. Focused on services developers can integrate today.

Maintained by [Backblaze](https://www.backblaze.com).

### Related Lists

- [Awesome Image Generation](https://github.com/backblaze-labs/awesome-image-generation)
- [Awesome Audio Generation](https://github.com/backblaze-labs/awesome-audio-generation)
- [Awesome ML Data Pipelines](https://github.com/backblaze-labs/awesome-ml-data-pipelines)
- [Awesome Multimodal Data](https://github.com/backblaze-labs/awesome-multimodal-data)
- [Awesome Agent Infrastructure](https://github.com/backblaze-labs/awesome-agent-infrastructure)
- [Awesome Physical AI](https://github.com/backblaze-labs/awesome-physical-ai)

## Contents

- [Text-to-Video APIs](#text-to-video-apis)
- [Real-Time and Interactive Video](#real-time-and-interactive-video)
- [Avatar and Talking Head APIs](#avatar-and-talking-head-apis)
- [Video Style Transfer and Motion](#video-style-transfer-and-motion)
- [Video Enhancement and Understanding](#video-enhancement-and-understanding)
- [Open Source Models](#open-source-models)
- [SDKs and Developer Tooling](#sdks-and-developer-tooling)
- [Infrastructure and Deployment](#infrastructure-and-deployment)
- [Evaluation and Observability](#evaluation-and-observability)
- [Templates and Example Projects](#templates-and-example-projects)

---

## Text-to-Video APIs

> Commercial text-to-video and image-to-video APIs with developer access.

- **[Stability AI (SVD)](https://huggingface.co/stabilityai/stable-video-diffusion-img2vid-xt)** – Image-to-video via Stable Video Diffusion. Hosted API deprecated July 2025; open weights available for self-hosting. [Docs](https://github.com/Stability-AI/generative-models)
- **[Fliki](https://fliki.ai)** – Text-to-video and text-to-speech platform. Enterprise API with 2,500+ voices in 80+ languages. [Docs](https://developer.fliki.ai)
- **[Google Veo 2 / Veo 3](https://deepmind.google/technologies/veo/)** – Google's video generation models via Vertex AI and Gemini API. Veo 2 is GA; Veo 3 in paid preview. [Docs](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/model-reference/veo-video-generation) | SDK: Google Cloud Python
- **[HappyHorse-1.0](https://happyhorse.app)** – Native 1080p text-to-video and image-to-video with integrated audio and lip-sync in one pass. Task-based REST with Bearer auth. [Docs](https://happyhorse.app/docs)
- **[Higgsfield](https://higgsfield.ai)** – Cinematic video platform aggregating 15+ premium models (Sora 2, Kling 2.6, Veo 3.1, etc.) with camera simulation, character consistency, and lip-sync. 15M+ users.
- **[InVideo AI](https://invideo.io)** – Turns text prompts into full videos using Sora 2 and Veo 3.1 as underlying models. OpenAI's first official Sora 2 integration partner. 50M+ users.
- **[Kling AI](https://klingai.com)** – Text-to-video and image-to-video from Kuaishou. Up to 30s clips at 1080p/30fps. Async task-based API. Also on fal.ai. [Docs](https://app.klingai.com/global/dev/document-api/quickStart/productIntroduction/overview)
- **[Krea](https://www.krea.ai/features/api)** – Unified API for 10+ video models (Veo 3/3.1, Sora 2, Kling 2.6, Wan 2.5, Hailuo 2.3, Runway Gen-4.5, Ray 2, Seedance Pro). Job-based with webhooks. OpenAPI spec, Python/Node/Go examples. [Docs](https://docs.krea.ai) | SDK: Python, Node, Go
- **[Leonardo.AI (Motion API)](https://leonardo.ai/api)** – Text-to-video and image-to-video REST API. Supports Motion 2.0, Veo 3, Veo 3 Fast, Kling 2.1/2.5 models. 480p–1080p, 4–8s clips, frame interpolation, style control. [Docs](https://docs.leonardo.ai/reference/createtexttovideogeneration)
- **[Luma Dream Machine](https://lumalabs.ai/dream-machine)** – High-quality text-to-video with character reference and style reference inputs. Ray 3 is the latest model. [Docs](https://docs.lumalabs.ai/docs/api) | SDK: [Python](https://github.com/lumalabs/lumaai-python), [JS](https://www.npmjs.com/package/lumaai)
- **[Magic Hour](https://magichour.ai)** – Multi-modal AI video generation API. Text-to-video, image-to-video, style transfer, 4K upscaling. Scales to zero when idle. [Docs](https://docs.magichour.ai)
- **[MiniMax / Hailuo](https://www.minimax.io)** – Hailuo 2.3 model. Text-to-video and image-to-video up to 1080p, 10s clips. [Docs](https://platform.minimax.io/docs/guides/video-generation) | SDK: [Python](https://pypi.org/project/minimax/), [Node](https://www.npmjs.com/package/minimax)
- **[Morph Studio](https://www.morphstudio.com)** – No-code AI video studio aggregating Wan 2.6, Kling 2.6 Pro, Seedance, Sora 2, Veo 3 into a single canvas with storyboarding and style transfer.
- **[OpenAI Sora](https://openai.com/sora)** – Text-to-video and image-to-video via the v1/videos endpoint. Sora 2 supports up to 90s at 4K with spatial audio. [Docs](https://platform.openai.com/docs/api-reference/videos) | SDK: Python, Node
- **[Pika (v2.2)](https://pika.art/api)** – Text-to-video and image-to-video with Pikaframes multi-keyframe interpolation. API powered by fal.ai. [Docs](https://fal.ai/models/fal-ai/pika/v2.2/text-to-video/api) | SDK: fal Python, fal JS
- **[Runway (Gen-4)](https://runwayml.com/api)** – Text-to-video and image-to-video with Gen-4 Turbo. Async task-based REST API with polling helpers. [Docs](https://docs.dev.runwayml.com) | SDK: [Python](https://pypi.org/project/runwayml/), [Node](https://github.com/runwayml/sdk-node)
- **[Seedance 2.0 (ByteDance)](https://seed.bytedance.com/en/seedance2_0)** – Dual-Branch Diffusion Transformer for simultaneous video + audio generation. Up to 15s at 2K resolution. Available via Dreamina. [Docs](https://dreamina.capcut.com)
- **[Vidu (Shengshu Technology)](https://www.shengshu.com/en/vidu)** – Now on Vidu Q3, the first long-form AI video model with native audio-video generation in a single output. Ranked
- **[Wan 2.7 (Alibaba)](https://fal.ai/wan-2.7)** – Commercial successor to open-weight Wan 2.2. Native 1080p, 2–15s clips, first-and-last-frame control, up to 5 reference inputs, instruction-based video editing. Via DashScope and fal.ai at $0.10/sec. [Docs](https://help.aliyun.com/zh/model-studio/wanx-video-generation)
- **[xAI Aurora / Grok Imagine](https://x.ai)** – Text-to-video and image-to-video using xAI's Aurora autoregressive MoE model. 6–15s clips at 720p with synchronized audio. [Docs](https://x.ai/news/grok-imagine-api)

## Real-Time and Interactive Video

> Low-latency video transformation and interactive streaming platforms.

- **[Krea Realtime 14B](https://github.com/krea-ai/realtime-video)** – Open-weight 14B autoregressive video model distilled from Wan 2.1 via Self-Forcing. ~11fps on a single B200, ~1s time-to-first-frame. WebSocket streaming server for mid-generation prompt edits. Research/non-commercial license. [Docs](https://huggingface.co/krea/krea-realtime-video)
- **[Causal Forcing](https://github.com/thu-ml/Causal-Forcing)** – Autoregressive diffusion distillation for real-time interactive video generation on a single RTX 4090. Frame-wise and chunk-wise inference; builds on Wan 2.1. HuggingFace weights at zhuhz22/Causal-Forcing. [Docs](https://thu-ml.github.io/CausalForcing.github.io/)
- **[CausVid](https://github.com/tianweiy/CausVid)** – CVPR 2025. Distills a bidirectional video diffusion transformer into a 4-step autoregressive generator. Enables streaming video generation at 9.4 FPS on a single GPU via KV caching. Supports T2V, I2V, and video-to-video translation. [Docs](https://huggingface.co/tianweiy/CausVid)
- **[Decart (Lucy 2)](https://decart.ai)** – Real-time video transformation at 30fps 1080p with near-zero latency. Live-stream style transfer, character swaps, environment transformation, product placement. ~$3/hour. [Docs](https://docs.platform.decart.ai/models/video/video-generation)
- **[Helios (PKU Yuan Group)](https://github.com/PKU-YuanGroup/Helios)** – 14B autoregressive diffusion model for T2V, I2V, and V2V. Generates minute-scale video at 19.5 FPS on a single H100 without KV-cache or causal masking. Three weight variants (Base, Mid, Distilled) on HuggingFace. Diffusers-compatible; group offloading reduces VRAM to ~6 GB. [Docs](https://pku-yuangroup.github.io/Helios-Page/)
- **[HY-WorldPlay (Tencent)](https://github.com/Tencent-Hunyuan/HY-WorldPlay)** – Streaming video diffusion model for real-time interactive world generation at 24fps. Accepts image or text prompt; responds to keyboard/mouse camera inputs. WorldPlay-5B and 8B weights open. Built on HunyuanVideo 1.5. [Docs](https://huggingface.co/tencent/HY-WorldPlay)
- **[LongLive (NVIDIA Labs)](https://github.com/NVlabs/LongLive)** – ICLR 2026. Real-time interactive long video generation at 20.7 FPS on a single H100. Accepts sequential user prompts; generates up to 240s with visual consistency via KV-recache and frame-level attention sink. LongLive-1.3B weights on HuggingFace. [Docs](https://nvlabs.github.io/LongLive/)
- **[PixVerse](https://pixverse.ai)** – Text-to-video and image-to-video platform. PixVerse-R1 adds real-time interactive video at 720p HD with native audio. [Docs](https://docs.platform.pixverse.ai)

## Avatar and Talking Head APIs

> Avatar video generation, lip-sync, and real-time streaming avatars.

- **[Anam AI](https://anam.ai)** – Real-time interactive avatar API. CARA-3 model, 180ms median latency at 25fps/720x480. Connects to any LLM. JavaScript and Python SDKs. [Docs](https://anam.ai/api) | SDK: [JavaScript](https://github.com/anam-org/javascript-sdk), [Python](https://github.com/anam-org/python-sdk)
- **[Captions / Mirage](https://captions.ai)** – Mirage API generates hyperrealistic talking-head videos from script + image + actor ID. Natural gestures, eye contact, synchronized audio. [Docs](https://help.mirage.app/api-reference/api)
- **[Colossyan](https://www.colossyan.com)** – Enterprise avatar video platform. 130+ avatars, 600+ voices, 100+ languages, instant avatar creation from phone recording. [Docs](https://www.colossyan.com/api)
- **[D-ID](https://www.d-id.com/api/)** – Talking head video generation from text or audio. Express and Premium+ avatars, real-time WebRTC streaming. [Docs](https://docs.d-id.com/) | SDK: [Python](https://pypi.org/project/did-api/)
- **[DeepBrain AI (AI Studios)](https://www.deepbrain.io)** – AI avatar video platform with REST API. Integrates AWS, Azure, ElevenLabs, IBM Watson, NVIDIA Riva. [Docs](https://docs.aistudios.com)
- **[Elai.io](https://elai.io)** – AI video platform with streaming avatar API for interactive e-learning. Turns documents and scripts into avatar-presented videos. [Docs](https://elai.readme.io)
- **[Hedra](https://www.hedra.com)** – Character-3 omnimodal talking-avatar API (image + text + audio in one pass). Long-form up to 10 min; LiveKit plugin for realtime; Node SDK, REST, Make.com integration. Omnia Fast Alpha adds full scene control. [Docs](https://docs.hedra.com) | SDK: Node
- **[HeyGen](https://www.heygen.com)** – AI avatar video generation and real-time streaming avatars via WebRTC. Template-based workflows. [Docs](https://docs.heygen.com/) | SDK: [JS/TS](https://github.com/HeyGen-Official/StreamingAvatarSDK)
- **[Hour One](https://hourone.ai)** – AI avatar video generator with 100+ presenters, voice cloning, 100+ languages. API + Zapier integration.
- **[Simli](https://www.simli.com)** – Real-time speech-to-video avatar API using 3D Gaussian splatting for full-face animation (not just lip-sync). WebRTC streaming, <200ms latency. Python and JS SDKs. [Docs](https://docs.simli.com) | SDK: [Python](https://docs.simli.com/api-reference/python), [JavaScript](https://github.com/simliai/simli-client)
- **[Sync.so](https://sync.so)** – Studio-grade lipsync and visual dubbing API. sync-3 flagship at native 4K with obstruction detection; lipsync-2-pro for diffusion super-res; react-1 for expressive emotion. Batch up to 500 videos per job. From $0.02/sec. [Docs](https://sync.so/docs/introduction) | SDK: [Python](https://pypi.org/project/syncsdk/), [TypeScript](https://www.npmjs.com/package/@sync.so/sdk)
- **[Synthesia](https://www.synthesia.io)** – Avatar-based video creation from scripts. 140+ languages, custom avatars, template workflows. API in beta. [Docs](https://docs.synthesia.io/)
- **[SynthLife](https://synthlife.co)** – Virtual AI influencer creation. Creates AI personas for TikTok, YouTube, Instagram with auto-scheduling and unlimited content generation.
- **[Tavus](https://www.tavus.io)** – Conversational video AI. Phoenix-4 model does real-time gaussian-diffusion facial synthesis at ~600ms latency. Replica API clones face + voice. Integrates with Pipecat and LiveKit. [Docs](https://www.tavus.io/ai-video-api)
- **[VEED Fabric 1.0](https://www.veed.io/tools/fabric-1.0-api)** – Image + audio to talking-video API. Diffusion Transformer drives lip-sync, head, and body gestures from any image (photo, illustration, mascot). Up to 5 min; 480p/720p MP4 output. REST via fal.ai; Python and JS SDKs. [Docs](https://fal.ai/models/veed/fabric-1.0) | SDK: [Python](https://docs.fal.ai), [JavaScript](https://docs.fal.ai)

## Video Style Transfer and Motion

> Video-to-video restyling and motion-transfer tools.

- **[DomoAI](https://www.domoai.app)** – AI video-to-video style remixer. 50+ styles (anime, Ghibli, cinematic). v2.4.1 supports text-to-video, image-to-video, talking avatars, and animation.
- **[Viggle AI](https://viggle.ai)** – Motion-transfer video tool that animates static characters to match a motion video or live webcam input. Mix Mode, Live Mode, and VTubing support. 40M+ users.

## Video Enhancement and Understanding

> Upscaling, restoration, and multimodal understanding APIs for video.

- **[FlashVSR](https://github.com/OpenImagingLab/FlashVSR)** – CVPR 2026. One-step diffusion framework for streaming 4x video super-resolution at ~17 FPS for 768x1408 on a single A100. Locality-constrained sparse attention and tiny conditional decoder. Apache-2.0; v1.1 weights on HuggingFace. [Docs](https://huggingface.co/JunhaoZhuang/FlashVSR-v1.1)
- **[REAL Video Enhancer](https://github.com/TNTwise/REAL-Video-Enhancer)** – Cross-platform GUI/CLI for frame interpolation (RIFE), upscaling (Real-ESRGAN, Waifu2x), denoising, and decompression. TensorRT and NCNN backends. Windows/macOS/Linux; v2.4.1 released Jan 2026.
- **[Topaz Video AI](https://www.topazlabs.com/topaz-video)** – AI video upscaling, denoising, frame interpolation, and artifact correction. 3M+ users; used by Google, Tesla, NASA. [Docs](https://developer.topazlabs.com)
- **[Twelve Labs](https://www.twelvelabs.io)** – Video understanding and intelligence API. Multimodal semantic search, analysis, and text generation from video content. [Docs](https://docs.twelvelabs.io)
- **[Video2X](https://github.com/k4yt3x/video2x)** – C/C++ framework for AI video super-resolution and frame interpolation. Supports Real-ESRGAN, Real-CUGAN, and RIFE via Vulkan. GUI and CLI. Docker images on GHCR. [Docs](https://github.com/k4yt3x/video2x/wiki)
- **[WebSR](https://github.com/sb2702/websr)** – JavaScript/WebGPU library for real-time AI video and image upscaling in the browser. Multiple pre-trained network sizes (animation, real-life, 3D content), worker thread support, and a custom training pipeline. Installable via npm. SDK: [JavaScript](https://www.npmjs.com/package/@websr/websr)

## Open Source Models

> Open-weight video models with hosted inference, Docker, or diffusers support.

- **[Open-Sora](https://github.com/hpcaitech/Open-Sora)** – Open reproduction of Sora-like generation. 2s–15s at 144p–720p. T2V, I2V, V2V.
- **[Wan 2.1 (Alibaba)](https://github.com/Wan-Video/Wan2.1)** – SOTA open T2V-14B model. Also supports I2V, editing, T2I, and V2A. T2V-1.3B runs on consumer GPUs. Also on Replicate and fal.ai. [Docs](https://huggingface.co/Wan-AI/Wan2.1-T2V-14B)
- **[Wan 2.2 (Alibaba)](https://github.com/Wan-Video/Wan2.2)** – First open-source MoE video diffusion model. +65.6% more image training data and +83.2% more video data vs 2.1. 5B and 14B variants. [Docs](https://huggingface.co/Wan-AI/Wan2.2-T2V-A14B)
- **[CogVideoX (Zhipu AI / Z.AI)](https://github.com/zai-org/CogVideo)** – CogVideoX-5B flagship; supports 10s videos. Commercial product "Ying" available via API. [Docs](https://huggingface.co/zai-org/CogVideoX-5b)
- **[AnimateDiff](https://github.com/guoyww/AnimateDiff)** – Plug-and-play animation module for Stable Diffusion models. Merged into HuggingFace diffusers. [Docs](https://huggingface.co/docs/diffusers/api/pipelines/animatediff)
- **[HunyuanVideo (Tencent)](https://github.com/Tencent-Hunyuan/HunyuanVideo)** – 13B+ param model; v1.5 is 8.3B and runs on consumer GPUs. I2V, Avatar, and Foley variants available. On Replicate and fal.ai. [Docs](https://github.com/Tencent-Hunyuan/HunyuanVideo-1.5)
- **[LTX-Video / LTX-2 (Lightricks)](https://github.com/Lightricks/LTX-Video)** – First DiT-based real-time video gen model. LTX-2 adds native 4K at 50fps with synchronized audio. ComfyUI nodes available. [Docs](https://github.com/Lightricks/LTX-2)
- **[SkyReels (SkyworkAI)](https://github.com/SkyworkAI/SkyReels-V2)** – V1: human-centric video fine-tuned on HunyuanVideo. V2: infinite-length video via Autoregressive Diffusion-Forcing. V3: multimodal reaching closed-source SOTA levels. [Docs](https://github.com/SkyworkAI/SkyReels-V3)
- **[MAGI-1 (Sand AI)](https://github.com/SandAI-org/MAGI-1)** – 24B param autoregressive denoising model. Generates video chunk-by-chunk (24 frames/chunk). T2V, I2V, V2V with streaming generation. Outperforms Wan 2.1 and HunyuanVideo on benchmarks. [Docs](https://huggingface.co/sand-ai/MAGI-1)
- **[Step-Video-T2V (StepFun)](https://github.com/stepfun-ai/Step-Video-T2V)** – 300B parameter text-to-video model, up to 204 frames, bilingual (EN/ZH). [Docs](https://huggingface.co/stepfun-ai/stepvideo-t2v)
- **[Pyramid Flow](https://github.com/jy0205/Pyramid-Flow)** – Efficient autoregressive video generation using pyramidal flow matching. Up to 10s at 768p, 24fps. ICLR 2025. [Docs](https://huggingface.co/rain1011/pyramid-flow-sd3)
- **[LongCat-Video (Meituan)](https://github.com/meituan-longcat/LongCat-Video)** – 13.6B foundation model for text-to-video, image-to-video, and video continuation, tuned for efficient long-form 720p generation. FlashAttention-2 acceleration. Streamlit demo included. Avatar variant released Dec 2025. [Docs](https://huggingface.co/meituan-longcat)
- **[OmniAvatar](https://github.com/Omni-Avatar/OmniAvatar)** – Audio-driven full-body avatar video generation with adaptive body animation. Pixel-wise multi-hierarchical audio embedding for diverse scenes. 1.3B and 14B variants (LoRA on Wan 2.1). Local inference via CLI. [Docs](https://omni-avatar.github.io)
- **[Allegro (Rhymes AI)](https://github.com/rhymes-ai/Allegro)** – 2.8B param VideoDiT. 6s clips at 720p/15fps. Merged into diffusers. [Docs](https://huggingface.co/rhymes-ai/Allegro)
- **[MOVA (OpenMOSS)](https://github.com/OpenMOSS/MOVA)** – Open foundation model for synchronized video+audio generation in a single inference pass. Asymmetric dual-tower architecture with cross-attention fusion. Multilingual lip-sync and environment-aware SFX. 360p and 720p weights. Diffusers integration planned. [Docs](https://huggingface.co/OpenMOSS-Team/MOVA-720p)
- **[daVinci-MagiHuman](https://github.com/GAIR-NLP/daVinci-MagiHuman)** – 15B open-source audio-video generation model (Sand.ai + GAIR). Unified transformer jointly processes text, video, and audio for lip-synced talking-head generation. T2V and TI2V modes; 7 languages; 2s for 5s/256p clip on H100. Apache-2.0. [Docs](https://huggingface.co/GAIR/daVinci-MagiHuman)
- **[Duix Avatar](https://github.com/duixcom/Duix-Avatar)** – Offline AI avatar video toolkit. Clone appearance and voice to create digital humans, then drive them via text or audio. Fully offline; Windows and Ubuntu support. Free commercial use under community license. [Docs](https://github.com/duixcom/Duix-Avatar/wiki)
- **[EchoMimicV2 (Ant Group)](https://github.com/antgroup/echomimic_v2)** – CVPR 2025. Audio-driven semi-body human animation from a single image + audio. Supports English and Mandarin. Accelerated inference (~50s for 120 frames on A100). Gradio UI included. [Docs](https://huggingface.co/BadToBest/EchoMimicV2)
- **[FramePack (lllyasviel)](https://github.com/lllyasviel/FramePack)** – Next-frame prediction I2V model that packs input context to constant length so generation cost is independent of video length. Generates 60s/30fps video with a 13B model on 6 GB VRAM. Gradio GUI; Windows one-click package and Linux pip install. [Docs](https://lllyasviel.github.io/frame_pack_gitpage/)
- **[LivePortrait (KwaiVGI)](https://github.com/KwaiVGI/LivePortrait)** – Efficient portrait animation via stitching and retargeting control. 12.8ms/frame on RTX 4090. Humans and Animals modes. Gradio UI and HuggingFace Space. [Docs](https://liveportrait.github.io)
- **[Meta Movie Gen](https://ai.meta.com/research/movie-gen/)** – 30B param T2V + 13B audio model. Personalized video from single reference photo, local/global editing, synchronized audio. Research paper public; weights not yet released. Rolling out inside Instagram Reels.
- **[Mochi 1 (Genmo)](https://www.genmo.ai)** – 10B param T2V model with AsymmDiT architecture. 5.4s at 30fps. On fal.ai and Replicate.
- **[MuseTalk (Tencent Music)](https://github.com/TMElyralab/MuseTalk)** – Real-time audio-driven lip-sync in latent space. 30fps+ on a V100. v1.5 improves identity consistency. Supports Chinese, English, and Japanese. [Docs](https://huggingface.co/TMElyralab/MuseTalk)
- **[NVIDIA Cosmos](https://github.com/nvidia-cosmos)** – World foundation model for physical AI (robotics, autonomous vehicles). Cosmos-Predict2.5 generates physics-based video simulations from text/image/video/sensor inputs. [Docs](https://docs.nvidia.com/cosmos/latest/introduction.html)
- **[OmniHuman-1 (ByteDance)](https://omnihuman-lab.github.io)** – Multimodal human video generation from single image + motion signal (audio, video, or text). Full-body, any aspect ratio. On Replicate.
- **[Open-Sora-Plan (PKU Yuan Group)](https://github.com/PKU-YuanGroup/Open-Sora-Plan)** – Open reproduction of Sora-style generation. v1.5.0 (Jun 2025) uses an 8B-scale sparse DiT (SUV) with WFVAE achieving HunyuanVideo-level quality. Supports T2V, I2V, and image generation. HuggingFace and ModelScope weights. [Docs](https://huggingface.co/PKU-Yuan-Lab)
- **[SkyReels-A2 (SkyworkAI)](https://github.com/SkyworkAI/SkyReels-A2)** – Elements-to-video (E2V) controllable generation framework. Compose arbitrary visual elements (characters, objects, backgrounds) from reference images into coherent video via text prompts. 14B Wan2.1-based weights on HuggingFace. ComfyUI-compatible; Gradio demo included. [Docs](https://huggingface.co/Skywork/SkyReels-A2)
- **[UniVidX](https://github.com/houyuanchen111/UniVidX)** – SIGGRAPH 2026. Unified multimodal video diffusion framework handling 15 tasks (T2V, V2V, intrinsic decomposition, alpha matting) from one model. Stochastic Condition Masking enables any-to-any conditioning. Built on Wan2.1-T2V-14B; Apache-2.0 weights on HuggingFace. [Docs](https://huggingface.co/houyuanchen111/UniVidX)
- **[Vid2World](https://github.com/thuml/Vid2World)** – ICLR 2026. Converts pretrained video diffusion models into action-conditioned interactive world models for robotics, game simulation, and navigation. Non-causal backbone is converted to autoregressive causal architecture with frame-level action conditioning. Pretrained checkpoints on HuggingFace. [Docs](https://knightnemo.github.io/vid2world/)
- **[Wan-Alpha](https://github.com/WeChatCV/Wan-Alpha)** – CVPR 2026 highlight. Text-to-video model that outputs video with transparent alpha channels via a Shiftable RGB-A Distribution Learner. Enables compositing with arbitrary backgrounds. v1.0 and v2.0 weights on HuggingFace; ComfyUI nodes available. [Docs](https://huggingface.co/htdong/Wan-Alpha)

## SDKs and Developer Tooling

> Client SDKs and libraries for integrating video generation into apps.

- **[HuggingFace Diffusers](https://github.com/huggingface/diffusers)** – The canonical PyTorch library for diffusion models including video pipelines. [Docs](https://huggingface.co/docs/diffusers) | SDK: Python (pip install diffusers)
- **[MiniMax MCP Server](https://github.com/MiniMax-AI/MiniMax-MCP)** – Model Context Protocol servers for video gen, TTS, and voice cloning. [Docs](https://github.com/MiniMax-AI/MiniMax-MCP-JS)
- **[Replicate SDK](https://github.com/replicate/replicate-python)** – Python/JS client for 100+ hosted video models. Async, streaming, webhooks, fine-tuning. [Docs](https://replicate.com/docs/get-started/python) | SDK: Python (pip install replicate)
- **[fal.ai SDK](https://github.com/fal-ai/fal-js)** – Serverless AI inference with Python, JS, and Swift SDKs. Hosts Kling, Veo, Pika, Wan, LTX, Luma, and more. [Docs](https://docs.fal.ai) | SDK: Python (pip install fal-client), Node (npm install @fal-ai/client)
- **[Luma AI SDK](https://github.com/lumalabs/lumaai-python)** – Sync and async clients for all Dream Machine generation modes. [Docs](https://docs.lumalabs.ai/docs/javascript) | SDK: Python (pip install lumaai)
- **[Creatomate](https://creatomate.com)** – Cloud video rendering API for generating data-driven videos from JSON templates. REST API with Node.js, PHP, and Python SDKs. Scales automatically; free trial available. [Docs](https://creatomate.com/docs/api/introduction) | SDK: [Node](https://github.com/Creatomate/creatomate-node), [PHP](https://packagist.org/packages/creatomate/creatomate), [JavaScript](https://github.com/Creatomate/creatomate-preview)
- **[FastVideo](https://github.com/hao-ai-lab/FastVideo)** – Unified post-training and inference framework for accelerating video diffusion models. pip install fastvideo. Supports Wan2.1/2.2 distillation; 3x speedup via SageAttention and Teacache. Scales to 64 GPUs. [Docs](https://hao-ai-lab.github.io/FastVideo/) | SDK: [Python](https://pypi.org/project/fastvideo/)
- **[HeyGen Streaming Avatar SDK](https://github.com/HeyGen-Official/StreamingAvatarSDK)** – TypeScript SDK for real-time WebRTC interactive avatar sessions. SDK: TypeScript (npm install @heygen/streaming-avatar)
- **[LTX Desktop](https://github.com/Lightricks/LTX-Desktop)** – Open-source nonlinear video editor with on-device AI generation (text-to-video, image-to-video, audio-to-video, retake). Runs locally on Windows/Linux with NVIDIA GPUs; API mode for macOS. Built on LTX-2.3. v1.0.5 released Apr 2026. [Docs](https://docs.ltx.video/open-source-model/getting-started/quick-start)
- **[rCM (NVIDIA Labs)](https://github.com/NVlabs/rcm)** – ICLR 2026. JVP-based continuous-time consistency distillation for 10B+ video diffusion models (Wan2.1, Cosmos-Predict2). Generates high-quality videos in 2–4 steps, 15–50x faster than full diffusion. FlashAttention-2 JVP kernel open-sourced.
- **[Remotion](https://www.remotion.dev)** – React framework for programmatic video generation. Define videos as React components, render server-side via CLI or Lambda (AWS). TypeScript-first; supports any CSS, Canvas, SVG, WebGL. [Docs](https://www.remotion.dev/docs) | SDK: [TypeScript](https://www.npmjs.com/package/remotion)
- **[Runway SDK](https://docs.dev.runwayml.com/api-details/sdks/)** – Official Python and Node.js SDKs with type annotations, async support, and built-in polling. SDK: Python (pip install runwayml), Node (npm install @runwayml/sdk)
- **[Shotstack](https://shotstack.io)** – Cloud video editing API. Render data-driven and AI-generated videos at scale via JSON templates. Node, Python, PHP, and Ruby SDKs. [Docs](https://shotstack.io/docs/guide/getting-started/core-concepts/) | SDK: [Node](https://github.com/shotstack/shotstack-sdk-node), [Python](https://github.com/shotstack/shotstack-sdk-python), [PHP](https://github.com/shotstack/shotstack-sdk-php), [Ruby](https://github.com/shotstack/shotstack-sdk-ruby)
- **[TalkingHead (met4citizen)](https://github.com/met4citizen/TalkingHead)** – JavaScript class for real-time 3D avatar lip-sync. Full-body RPM/VRM avatars driven by TTS audio. Integrates ElevenLabs, OpenAI, Google TTS, and Azure. Installable via npm; CDN import also supported. MIT license; v1.7.0 released Dec 2025. [Docs](https://met4citizen.github.io/TalkingHead/) | SDK: [JavaScript](https://www.npmjs.com/package/@met4citizen/talkinghead)
- **[TurboDiffusion](https://github.com/thu-ml/TurboDiffusion)** – Inference acceleration framework for video diffusion models. Combines SageAttention, Sparse-Linear Attention, and rCM timestep distillation for 100–200x speedup. Supports TurboWan 2.1/2.2 T2V and I2V at 480p/720p. pip install + CLI inference.
- **[Wan2GP](https://github.com/deepbeepmeep/Wan2GP)** – Low-VRAM inference GUI and server for Wan 2.1/2.2, HunyuanVideo, LTX-Video, and Flux. Runs on 6 GB VRAM via int8/fp8/GGUF/NV FP4 quantization. Supports AMD RDNA and older Nvidia GPUs. Gradio web UI with mask editor and motion designer. Custom community license; free for non-commercial use.

## Infrastructure and Deployment

> GPU platforms, video processing, storage and CDN, and playback libraries.

- **[HandBrake](https://handbrake.fr)** – Open-source video transcoder wrapping FFmpeg. GUI and CLI. [Docs](https://github.com/HandBrake/HandBrake)
- **[hls.js](https://github.com/video-dev/hls.js)** – JavaScript HLS playback via MSE. Used by major streaming platforms.
- **[Shaka Player](https://github.com/shaka-project/shaka-player)** – Google's open-source DASH + HLS player.
- **[Backblaze B2](https://www.backblaze.com/cloud-storage)** – S3-compatible object storage at low cost. Free egress via Cloudflare. [Docs](https://www.backblaze.com/docs/cloud-storage-s3-compatible-api) | [B2 integration](https://www.backblaze.com/docs/cloud-storage-s3-compatible-api)
- **[Cloudflare Stream](https://www.cloudflare.com/developer-platform/products/cloudflare-stream/)** – Video upload, encoding, and CDN delivery billed per minute watched. Live streaming via RTMP/SRT. [Docs](https://developers.cloudflare.com/stream/)
- **[CoreWeave](https://www.coreweave.com)** – Kubernetes-native AI cloud with enterprise-scale GPU infrastructure.
- **[fal.ai](https://fal.ai)** – Serverless inference for generative media. 600+ models. Python, JS, Swift SDKs. [Docs](https://docs.fal.ai)
- **[FFmpeg](https://ffmpeg.org)** – Industry-standard multimedia processing. Encode, decode, transcode, stream, filter. [Docs](https://github.com/FFmpeg/FFmpeg)
- **[Lambda Labs](https://lambdalabs.com)** – On-demand H100/B200 GPUs. SSH and JupyterLab access with REST API for instance management.
- **[Modal](https://modal.com)** – Serverless Python-first GPU platform. Container spin-up in ~1 second. [Docs](https://modal.com/docs/guide)
- **[Mux](https://www.mux.com)** – API-first video infrastructure. Upload, encode, stream (VOD + live), analytics. SDKs for Node, Python, Ruby, Go, and more. [Docs](https://docs.mux.com)
- **[Pollo AI](https://pollo.ai)** – Video API aggregator providing access to Kling, Veo 3.1, Runway, Hailuo, Wan 2.6, and Pollo 2.0. [Docs](https://docs.pollo.ai)
- **[Replicate](https://replicate.com)** – Serverless model hosting. Run open-source video models via REST API. [Docs](https://replicate.com/docs)
- **[RunPod](https://www.runpod.io)** – GPU pods (persistent) and serverless endpoints. REST, GraphQL, and CLI. [Docs](https://docs.runpod.io)
- **[SiliconFlow](https://siliconflow.cn)** – Managed inference API for open-source video models including Wan2.1/2.2 T2V and I2V, and HunyuanVideo-HD. OpenAI-compatible REST API at api.siliconflow.cn/v1. English docs available. [Docs](https://docs.siliconflow.cn/en/userguide/capabilities/video)
- **[Together AI](https://www.together.ai)** – Inference API for 200+ open models plus Instant Clusters for self-service GPU clusters.
- **[WaveSpeedAI](https://wavespeed.ai)** – Fast AI inference with no cold starts. 600+ models. 30–50% cheaper than HuggingFace Inference. 99.9% uptime SLA. [Docs](https://github.com/wavespeedai)

## Evaluation and Observability

> Benchmarks, leaderboards, and perceptual-quality metrics for video.

- **[VBench / VBench-2.0](https://github.com/Vchitect/VBench)** – Comprehensive benchmark for video generative models. 16 fine-grained dimensions including subject consistency, motion smoothness, temporal flickering. VBench-2.0 adds Physics and Commonsense evaluation. [Docs](https://huggingface.co/spaces/Vchitect/VBench_Leaderboard)
- **[Artificial Analysis Video Arena](https://artificialanalysis.ai/video/arena)** – Elo-based blind-comparison leaderboard for text-to-video and image-to-video models, with separate tracks for audio-enabled output. Embeddable leaderboard widgets and HuggingFace Space. [Docs](https://artificialanalysis.ai/video/leaderboard/text-to-video)

## Templates and Example Projects

> Reference implementations, demos, and starter projects.

- **[fal.ai Next.js Video Generator](https://github.com/fal-ai/fal-nextjs-template)** – Official Next.js template with queue management and TypeScript. One-click Vercel deploy. [Docs](https://vercel.com/templates/next.js/fal-video-generator)
- **[B2 Video Object Detection with Transformers](https://github.com/backblaze-b2-samples/b2-transformers-video-object-detection)** – Video object detection pipeline using HuggingFace Transformers with Backblaze B2 cloud storage integration. [B2 integration](https://github.com/backblaze-b2-samples/b2-transformers-video-object-detection)
- **[Google Gemini Streamlit + Cloud Run](https://github.com/GoogleCloudPlatform/generative-ai/tree/main/gemini/sample-apps/gemini-streamlit-cloudrun)** – Sample app using Gemini multimodal with Streamlit, deployable to Cloud Run.
- **[HeyGen Streaming Avatar Demo](https://github.com/HeyGen-Official/StreamingAvatarTSDemo)** – Next.js/TypeScript starter for real-time WebRTC avatar sessions.
- **[Pixelle-Video](https://github.com/AIDC-AI/Pixelle-Video)** – Fully-automated short video pipeline. Input a topic; the tool writes the script, generates AI images via ComfyUI, synthesizes voice (Edge-TTS/Index-TTS), adds music, and outputs a finished video. Supports GPT, Qwen, DeepSeek, and Ollama. Apache-2.0; v0.1.15 released Jan 2026. [Docs](https://aidc-ai.github.io/Pixelle-Video/)
- **[Stability AI SVD Streamlit Demo](https://github.com/Stability-AI/generative-models/tree/main/scripts/demo)** – Streamlit demo scripts for Stable Video Diffusion.

---

## Contributing

Contributions are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md). One entry per PR — edit `entries.yaml` only and let the maintainers regenerate `README.md`.

## License

Released under [CC0 1.0 Universal](LICENSE). You may copy, modify, and redistribute without attribution.

## About Backblaze B2

[Backblaze B2 Cloud Storage](https://www.backblaze.com/cloud-storage) is S3-compatible object storage designed for AI and media workloads. This list is maintained as part of our work making B2 a convenient storage layer for AI workflows.
