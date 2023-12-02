# Generative Models by Stability AI

This repo dose little optimization on Stable Video Diffusion inference.
I added Low VRAM mode by default from other demo, and it reduce VRAM usage ~30% for me (64GB RAM + RTX 3080Ti 12GB).

Now i can run SVD with 9 FPS and 18 Frames with in 1 minute without leaking too much VRAM to RAM; Also i can run SDXL-Turbo with no VRAM leak (fp16).

Launch SVD web app:
```shell
cd generative-models
streamlit run scripts/demo/video_sampling.py
```

Launch SDXL-Turbo or SD-Turbo web app:
```shell
cd generative-models
streamlit run scripts/demo/turbo.py