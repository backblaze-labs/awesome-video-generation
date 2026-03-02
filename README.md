# Awesome Video Generation [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com) [![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

A curated list of AI video generation APIs, SDKs, and production-ready tools.
Focused on services developers can integrate today.

> Last verified: March 2026

### Related Lists

- [Awesome Image Generation](../awesome-image-generation)
- [Awesome Audio Generation](../awesome-audio-generation)

---

## Contents

- [Text-to-Video APIs](#text-to-video-apis)
- [Real-Time and Interactive Video](#real-time-and-interactive-video)
- [Video Style Transfer and Motion](#video-style-transfer-and-motion)
- [Avatar and Talking Head APIs](#avatar-and-talking-head-apis)
- [Video Enhancement APIs](#video-enhancement-apis)
- [Video Understanding APIs](#video-understanding-apis)
- [Open Source Models](#open-source-models)
- [SDKs and Developer Tooling](#sdks-and-developer-tooling)
- [Infrastructure and Deployment](#infrastructure-and-deployment)
- [Evaluation and Observability](#evaluation-and-observability)
- [Templates and Example Projects](#templates-and-example-projects)
- [Learning Resources](#learning-resources)

---

## Text-to-Video APIs

- **[OpenAI Sora](https://openai.com/sora)** – Text-to-video and image-to-video via the `v1/videos` endpoint. Sora 2 supports up to 90s at 4K with spatial audio. [API Docs](https://platform.openai.com/docs/api-reference/videos) | SDK: Python, Node
- **[Runway (Gen-4)](https://runwayml.com/api)** – Text-to-video and image-to-video with Gen-4 Turbo. Async task-based REST API with polling helpers. [Docs](https://docs.dev.runwayml.com) | SDK: [Python](https://pypi.org/project/runwayml/), [Node](https://github.com/runwayml/sdk-node)
- **[Google Veo 2 / Veo 3](https://deepmind.google/technologies/veo/)** – Google's video generation models via Vertex AI and Gemini API. Veo 2 is GA; Veo 3 in paid preview. [Docs](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/model-reference/veo-video-generation) | SDK: Google Cloud Python
- **[Pika (v2.2)](https://pika.art/api)** – Text-to-video and image-to-video with Pikaframes multi-keyframe interpolation. API powered by fal.ai. [Docs](https://fal.ai/models/fal-ai/pika/v2.2/text-to-video/api) | SDK: fal Python, fal JS
- **[Luma Dream Machine](https://lumalabs.ai/dream-machine)** – High-quality text-to-video with character reference and style reference inputs. Ray 3 is the latest model. [Docs](https://docs.lumalabs.ai/docs/api) | SDK: [Python](https://github.com/lumalabs/lumaai-python), [JS](https://www.npmjs.com/package/lumaai)
- **[Kling AI](https://klingai.com)** – Text-to-video and image-to-video from Kuaishou. Up to 30s clips at 1080p/30fps. Async task-based API. [Docs](https://app.klingai.com/global/dev/document-api/quickStart/productIntroduction/overview) | Also on [fal.ai](https://fal.ai/kling-3)
- **[MiniMax / Hailuo](https://www.minimax.io)** – Hailuo 2.3 model. Text-to-video and image-to-video up to 1080p, 10s clips. [Docs](https://platform.minimax.io/docs/guides/video-generation) | SDK: [Python](https://pypi.org/project/minimax/), [Node](https://www.npmjs.com/package/minimax)
- **[Vidu (Shengshu Technology)](https://www.shengshu.com/en/vidu)** – Now on Vidu Q3, the first long-form AI video model with native audio-video generation in a single output. Ranked #2 globally on Artificial Analysis benchmarks.
- **[xAI Aurora / Grok Imagine](https://x.ai)** – Text-to-video and image-to-video using xAI's Aurora autoregressive MoE model. 6–15s clips at 720p with synchronized audio. [API](https://x.ai/news/grok-imagine-api)
- **[Seedance 2.0 (ByteDance)](https://seed.bytedance.com/en/seedance2_0)** – Dual-Branch Diffusion Transformer for simultaneous video + audio generation. Up to 15s at 2K resolution. Available via [Dreamina](https://dreamina.capcut.com).
- **[Stability AI (SVD)](https://huggingface.co/stabilityai/stable-video-diffusion-img2vid-xt)** – Image-to-video via Stable Video Diffusion. Hosted API deprecated July 2025; open weights available for self-hosting. [GitHub](https://github.com/Stability-AI/generative-models)
- **[Higgsfield](https://higgsfield.ai)** – Cinematic video platform aggregating 15+ premium models (Sora 2, Kling 2.6, Veo 3.1, etc.) with camera simulation, character consistency, and lip-sync. 15M+ users.
- **[Magic Hour](https://magichour.ai)** – Multi-modal AI video generation API. Text-to-video, image-to-video, style transfer, 4K upscaling. Scales to zero when idle. [Docs](https://docs.magichour.ai) | [API](https://magichour.ai/api)
- **[InVideo AI](https://invideo.io)** – Turns text prompts into full videos using Sora 2 and Veo 3.1 as underlying models. OpenAI's first official Sora 2 integration partner. 50M+ users.
- **[Fliki](https://fliki.ai)** – Text-to-video and text-to-speech platform. Enterprise API with 2,500+ voices in 80+ languages. [Docs](https://developer.fliki.ai)
- **[Morph Studio](https://www.morphstudio.com)** – No-code AI video studio aggregating Wan 2.6, Kling 2.6 Pro, Seedance, Sora 2, Veo 3 into a single canvas with storyboarding and style transfer.

## Real-Time and Interactive Video

- **[Decart (Lucy 2)](https://decart.ai)** – Real-time video transformation at 30fps 1080p with near-zero latency. Live-stream style transfer, character swaps, environment transformation, product placement. ~$3/hour. [Docs](https://docs.platform.decart.ai/models/video/video-generation) | [Platform](https://mirage.decart.ai)
- **[PixVerse](https://pixverse.ai)** – Text-to-video and image-to-video platform. PixVerse-R1 adds real-time interactive video at 720p HD with native audio. [Platform](https://platform.pixverse.ai) | [Docs](https://docs.platform.pixverse.ai)

## Video Style Transfer and Motion

- **[DomoAI](https://www.domoai.app)** – AI video-to-video style remixer. 50+ styles (anime, Ghibli, cinematic). v2.4.1 supports text-to-video, image-to-video, talking avatars, and animation.
- **[Viggle AI](https://viggle.ai)** – Motion-transfer video tool that animates static characters to match a motion video or live webcam input. Mix Mode, Live Mode, and VTubing support. 40M+ users.

## Avatar and Talking Head APIs

- **[Synthesia](https://www.synthesia.io)** – Avatar-based video creation from scripts. 140+ languages, custom avatars, template workflows. API in beta. [Docs](https://docs.synthesia.io/)
- **[D-ID](https://www.d-id.com/api/)** – Talking head video generation from text or audio. Express and Premium+ avatars, real-time WebRTC streaming. [Docs](https://docs.d-id.com/) | SDK: [Python](https://pypi.org/project/did-api/)
- **[HeyGen](https://www.heygen.com)** – AI avatar video generation and real-time streaming avatars via WebRTC. Template-based workflows. [Docs](https://docs.heygen.com/) | SDK: [JS/TS](https://github.com/HeyGen-Official/StreamingAvatarSDK)
- **[Tavus](https://www.tavus.io)** – Conversational video AI. Phoenix-4 model does real-time gaussian-diffusion facial synthesis at ~600ms latency. Replica API clones face + voice. Integrates with Pipecat and LiveKit. [Avatar API](https://www.tavus.io/avatar-api) | [Video API](https://www.tavus.io/ai-video-api)
- **[Colossyan](https://www.colossyan.com)** – Enterprise avatar video platform. 130+ avatars, 600+ voices, 100+ languages, instant avatar creation from phone recording. [API](https://www.colossyan.com/api)
- **[DeepBrain AI (AI Studios)](https://www.deepbrain.io)** – AI avatar video platform with REST API. Integrates AWS, Azure, ElevenLabs, IBM Watson, NVIDIA Riva. [Docs](https://docs.aistudios.com)
- **[Hour One](https://hourone.ai)** – AI avatar video generator with 100+ presenters, voice cloning, 100+ languages. API + Zapier integration.
- **[Elai.io](https://elai.io)** – AI video platform with streaming avatar API for interactive e-learning. Turns documents and scripts into avatar-presented videos. [Docs](https://elai.readme.io)
- **[Captions / Mirage](https://captions.ai)** – Mirage API generates hyperrealistic talking-head videos from script + image + actor ID. Natural gestures, eye contact, synchronized audio. [API](https://www.captions.ai/api) | [Docs](https://help.mirage.app/api-reference/api)
- **[SynthLife](https://synthlife.co)** – Virtual AI influencer creation. Creates AI personas for TikTok, YouTube, Instagram with auto-scheduling and unlimited content generation.

## Video Enhancement APIs

- **[Topaz Video AI](https://www.topazlabs.com/topaz-video)** – AI video upscaling, denoising, frame interpolation, and artifact correction. 3M+ users; used by Google, Tesla, NASA. [API](https://www.topazlabs.com/api) | [Docs](https://developer.topazlabs.com)

## Video Understanding APIs

- **[Twelve Labs](https://www.twelvelabs.io)** – Video understanding and intelligence API. Multimodal semantic search, analysis, and text generation from video content. [Docs](https://docs.twelvelabs.io)

## Open Source Models

Models with hosted inference, Docker support, or `diffusers` integration.

- **[Wan 2.1 (Alibaba)](https://github.com/Wan-Video/Wan2.1)** – SOTA open T2V-14B model. Also supports I2V, editing, T2I, and V2A. T2V-1.3B runs on consumer GPUs. Apache 2.0. [HuggingFace](https://huggingface.co/Wan-AI/Wan2.1-T2V-14B) | On [Replicate](https://replicate.com/collections/wan-video), [fal.ai](https://fal.ai/models/fal-ai/wan-i2v)
- **[Wan 2.2 (Alibaba)](https://github.com/Wan-Video/Wan2.2)** – World's first open-source MoE video diffusion model. +65.6% more image training data and +83.2% more video data vs 2.1. 5B and 14B variants. Apache 2.0. [HuggingFace](https://huggingface.co/Wan-AI/Wan2.2-T2V-A14B)
- **[MAGI-1 (Sand AI)](https://github.com/SandAI-org/MAGI-1)** – 24B param autoregressive denoising model. Generates video chunk-by-chunk (24 frames/chunk). Supports T2V, I2V, V2V with streaming generation. Outperforms Wan 2.1 and HunyuanVideo on benchmarks. Apache 2.0. [HuggingFace](https://huggingface.co/sand-ai/MAGI-1) | [Paper](https://arxiv.org/abs/2505.13211)
- **[Step-Video-T2V (StepFun)](https://github.com/stepfun-ai/Step-Video-T2V)** – 300B parameter text-to-video model, up to 204 frames, bilingual (EN/ZH). MIT license. [TI2V](https://github.com/stepfun-ai/Step-Video-TI2V) | [HuggingFace](https://huggingface.co/stepfun-ai/stepvideo-t2v)
- **[SkyReels (SkyworkAI)](https://github.com/SkyworkAI/SkyReels-V2)** – V1: human-centric video fine-tuned on HunyuanVideo. V2: infinite-length video via Autoregressive Diffusion-Forcing. V3: multimodal reaching closed-source SOTA levels. [V1](https://github.com/SkyworkAI/SkyReels-V1) | [V3](https://github.com/SkyworkAI/SkyReels-V3)
- **[HunyuanVideo (Tencent)](https://github.com/Tencent-Hunyuan/HunyuanVideo)** – 13B+ param model; v1.5 is 8.3B and runs on consumer GPUs. I2V, Avatar, and Foley variants available. [v1.5](https://github.com/Tencent-Hunyuan/HunyuanVideo-1.5) | On Replicate, fal.ai
- **[CogVideoX (Zhipu AI / Z.AI)](https://github.com/zai-org/CogVideo)** – CogVideoX-5B flagship; supports 10s videos. Commercial product "Ying" available via API. Apache 2.0 (2B). [HuggingFace](https://huggingface.co/zai-org/CogVideoX-5b) | [API](https://bigmodel.cn)
- **[NVIDIA Cosmos](https://github.com/nvidia-cosmos)** – World foundation model for physical AI (robotics, autonomous vehicles). Cosmos-Predict2.5 generates physics-based video simulations from text/image/video/sensor inputs. [Website](https://www.nvidia.com/en-us/ai/cosmos/) | [Docs](https://docs.nvidia.com/cosmos/latest/introduction.html)
- **[Meta Movie Gen](https://ai.meta.com/research/movie-gen/)** – 30B param T2V + 13B audio model. Personalized video from single reference photo, local/global editing, synchronized audio. Research paper public; weights not yet released. Rolling out inside Instagram Reels.
- **[LTX-Video / LTX-2 (Lightricks)](https://github.com/Lightricks/LTX-Video)** – First DiT-based real-time video gen model. LTX-2 adds native 4K at 50fps with synchronized audio. [LTX-2](https://github.com/Lightricks/LTX-2) | [ComfyUI Nodes](https://github.com/Lightricks/ComfyUI-LTXVideo)
- **[Pyramid Flow](https://github.com/jy0205/Pyramid-Flow)** – Efficient autoregressive video generation using pyramidal flow matching. Up to 10s at 768p, 24fps. ICLR 2025. [HuggingFace](https://huggingface.co/rain1011/pyramid-flow-sd3) | [Paper](https://arxiv.org/abs/2410.05954)
- **[Open-Sora](https://github.com/hpcaitech/Open-Sora)** – Open reproduction of Sora-like generation. 2s–15s at 144p–720p. T2V, I2V, V2V. Apache 2.0.
- **[AnimateDiff](https://github.com/guoyww/AnimateDiff)** – Plug-and-play animation module for Stable Diffusion models. Merged into HuggingFace diffusers. [Diffusers Docs](https://huggingface.co/docs/diffusers/api/pipelines/animatediff) | On [Replicate](https://replicate.com/lucataco/animate-diff)
- **[Mochi 1 (Genmo)](https://www.genmo.ai)** – 10B param T2V model with AsymmDiT architecture. 5.4s at 30fps. Apache 2.0. On fal.ai, Replicate
- **[Allegro (Rhymes AI)](https://github.com/rhymes-ai/Allegro)** – 2.8B param VideoDiT. 6s clips at 720p/15fps. Merged into diffusers. Apache 2.0. [HuggingFace](https://huggingface.co/rhymes-ai/Allegro)
- **[OmniHuman-1 (ByteDance)](https://omnihuman-lab.github.io)** – Multimodal human video generation from single image + motion signal (audio, video, or text). Full-body, any aspect ratio. On [Replicate](https://replicate.com/bytedance/omni-human)

## SDKs and Developer Tooling

- **[Replicate SDK](https://github.com/replicate/replicate-python)** – Python/JS client for 100+ hosted video models. Async, streaming, webhooks, fine-tuning. [Docs](https://replicate.com/docs/get-started/python) | `pip install replicate`
- **[fal.ai SDK](https://fal.ai)** – Serverless AI inference with Python, JS, and Swift SDKs. Hosts Kling, Veo, Pika, Wan, LTX, Luma, and more. [Docs](https://docs.fal.ai) | `pip install fal-client` / `npm install @fal-ai/client`
- **[Runway SDK](https://docs.dev.runwayml.com/api-details/sdks/)** – Official Python and Node.js SDKs with type annotations, async support, and built-in polling. `pip install runwayml` / `npm install @runwayml/sdk`
- **[Luma AI SDK](https://github.com/lumalabs/lumaai-python)** – Sync and async clients for all Dream Machine generation modes. [JS Docs](https://docs.lumalabs.ai/docs/javascript) | `pip install lumaai`
- **[HeyGen Streaming Avatar SDK](https://github.com/HeyGen-Official/StreamingAvatarSDK)** – TypeScript SDK for real-time WebRTC interactive avatar sessions. `npm install @heygen/streaming-avatar`
- **[MiniMax MCP Server](https://github.com/MiniMax-AI/MiniMax-MCP)** – Model Context Protocol servers for video gen, TTS, and voice cloning. [JS](https://github.com/MiniMax-AI/MiniMax-MCP-JS)
- **[HuggingFace Diffusers](https://github.com/huggingface/diffusers)** – The canonical PyTorch library for diffusion models including video pipelines. [Docs](https://huggingface.co/docs/diffusers) | `pip install diffusers`

## Infrastructure and Deployment

### GPU Cloud and Inference Platforms

- **[Lambda Labs](https://lambdalabs.com)** – On-demand H100/B200 GPUs. SSH and JupyterLab access with REST API for instance management.
- **[CoreWeave](https://www.coreweave.com)** – Kubernetes-native AI cloud with enterprise-scale GPU infrastructure.
- **[RunPod](https://www.runpod.io)** – GPU pods (persistent) and serverless endpoints. REST, GraphQL, and CLI. [Docs](https://docs.runpod.io)
- **[Modal](https://modal.com)** – Serverless Python-first GPU platform. Container spin-up in ~1 second. [Docs](https://modal.com/docs/guide)
- **[Together AI](https://www.together.ai)** – Inference API for 200+ open models plus Instant Clusters for self-service GPU clusters.
- **[Replicate](https://replicate.com)** – Serverless model hosting. Run open-source video models via REST API. [Docs](https://replicate.com/docs)
- **[fal.ai](https://fal.ai)** – Serverless inference for generative media. 600+ models. Python, JS, Swift SDKs. [Docs](https://docs.fal.ai)
- **[WaveSpeedAI](https://wavespeed.ai)** – Fast AI inference with no cold starts. 600+ models. 30–50% cheaper than HuggingFace Inference. 99.9% uptime SLA. [GitHub](https://github.com/wavespeedai)
- **[Pollo AI](https://pollo.ai)** – Video API aggregator providing access to Kling, Veo 3.1, Runway, Hailuo, Wan 2.6, and Pollo 2.0. [Docs](https://docs.pollo.ai) | [API](https://pollo.ai/api-platform)

### Video Processing

- **[FFmpeg](https://ffmpeg.org)** – Industry-standard multimedia processing. Encode, decode, transcode, stream, filter. [GitHub](https://github.com/FFmpeg/FFmpeg)
- **[HandBrake](https://handbrake.fr)** – Open-source video transcoder wrapping FFmpeg. GUI and CLI. [GitHub](https://github.com/HandBrake/HandBrake)

### Media Storage and Delivery

- **[Mux](https://www.mux.com)** – API-first video infrastructure. Upload, encode, stream (VOD + live), analytics. SDKs for Node, Python, Ruby, Go, and more. [Docs](https://docs.mux.com)
- **[Cloudflare Stream](https://www.cloudflare.com/developer-platform/products/cloudflare-stream/)** – Video upload, encoding, and CDN delivery billed per minute watched. Live streaming via RTMP/SRT. [Docs](https://developers.cloudflare.com/stream/)
- **[Backblaze B2](https://www.backblaze.com/cloud-storage)** – S3-compatible object storage at ~$0.006/GB/month. Free egress via Cloudflare. [Docs](https://www.backblaze.com/docs/cloud-storage-s3-compatible-api)

### Video Playback

- **[hls.js](https://github.com/video-dev/hls.js)** – JavaScript HLS playback via MSE. Used by major streaming platforms.
- **[Shaka Player](https://github.com/shaka-project/shaka-player)** – Google's open-source DASH + HLS player.

## Evaluation and Observability

- **[VBench / VBench-2.0](https://github.com/Vchitect/VBench)** – Comprehensive benchmark for video generative models. 16 fine-grained dimensions including subject consistency, motion smoothness, temporal flickering. VBench-2.0 adds Physics and Commonsense evaluation. [Leaderboard](https://huggingface.co/spaces/Vchitect/VBench_Leaderboard) | [Paper (CVPR 2024)](https://arxiv.org/abs/2311.17982)

## Templates and Example Projects

- **[fal.ai Next.js Video Generator](https://github.com/fal-ai/fal-nextjs-template)** – Official Next.js template with queue management and TypeScript. One-click Vercel deploy. [Vercel Template](https://vercel.com/templates/next.js/fal-video-generator)
- **[HeyGen Streaming Avatar Demo](https://github.com/HeyGen-Official/StreamingAvatarTSDemo)** – Next.js/TypeScript starter for real-time WebRTC avatar sessions.
- **[Stability AI SVD Streamlit Demo](https://github.com/Stability-AI/generative-models)** – Streamlit demo scripts for Stable Video Diffusion. (see `scripts/demo/`)
- **[B2 Video Object Detection with Transformers](https://github.com/backblaze-b2-samples/b2-transformers-video-object-detection)** – Video object detection pipeline using HuggingFace Transformers with Backblaze B2 cloud storage integration.
- **[Google Gemini Streamlit + Cloud Run](https://github.com/GoogleCloudPlatform/generative-ai/tree/main/gemini/sample-apps/gemini-streamlit-cloudrun)** – Sample app using Gemini multimodal with Streamlit, deployable to Cloud Run.

## Learning Resources

- [OpenAI Videos API Reference](https://platform.openai.com/docs/api-reference/videos)
- [Runway API Quickstart](https://docs.dev.runwayml.com)
- [Google Veo Developer Guide](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/models/veo/2-0-generate)
- [Luma AI API Docs](https://docs.lumalabs.ai/docs/api)
- [HuggingFace Diffusers Video Pipeline Guide](https://huggingface.co/docs/diffusers/api/pipelines/animatediff)
- [fal.ai Documentation](https://docs.fal.ai)
- [NVIDIA Cosmos Documentation](https://docs.nvidia.com/cosmos/latest/introduction.html)

---

## Contributing

Contributions welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first. PRs for new tools, corrections, and updates are appreciated.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
