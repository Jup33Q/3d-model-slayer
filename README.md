# 3D Model Slayer

Holographic quilt gallery + full pipeline documentation: **Draw Things image generation → MiniMax H3 FL2VA video → Looking Glass quilts**.

**Live site: https://jup33q.github.io/3d-model-slayer/**

## Contents

- **Holographic gallery** — interactive Looking Glass Blocks embeds (drag / move your head; true glasses-free 3D on LKG devices):
  - 白丝少女 · 序列重置 (2026-10-03, H3 FL2VA 56f, watercolor-Mucha → realistic)
  - 水墨白丝少女 (2026-10-02)
  - 蒸汽朋克塔奇克马 · 彩铅版 / 写实版 (2026-10-02)
- **Featured project** (videos/01 reset): final first/last frames, 56-frame video, 7×8 quilt image
- **Pipeline docs** — complete, re-runnable recipes for all three stages:
  - Stage B1: Qwen Image 2.1 four-slot canvas (color 32 / depth 45 / paper texture 7 / Mucha style 12)
  - Stage B2: realistic tail frame, two-slot canvas + Opaque Pantyhose & Ricklistic LoRAs
  - Stage C: MiniMax H3 FL2VA 56-frame six-section prompt (style ramp woven into the timeline)
- **Lessons learned** — dynamic-reference fabric pollution, Generation-mode-is-not-outpainting, temporal quilts vs true angular quilts, and more

## Tech stack

- Image: Draw Things (Qwen Image 2.1 / FLUX.2 klein / Illustrious XL), DA3Depth-ShaderEdit for 2.5D yaw reprojection (±5° parallax arc)
- Video: MiniMax H3 FL2VA (Edit mode), 56 frames @24fps, H3 Turbo 4-step LoRA
- Display: Looking Glass Go (`_qs…a0.56` quilts), hosted on [Looking Glass Blocks](https://blocks.glass)

## Repo layout

```
index.html      # single-page site (self-contained CSS, no build step)
assets/         # final frames, video, quilt image
LICENSE         # MIT (code)
LICENSE-CONTENT # CC0 1.0 (images / artwork)
```

## License

- Code (HTML/CSS): [MIT](LICENSE)
- Images & artwork: [CC0 1.0](LICENSE-CONTENT)
