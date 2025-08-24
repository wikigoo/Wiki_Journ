# 1) Purpose

Produce **one JSON object** that fully specifies a text-to-image request. The schema is compact, unambiguous, and tuned for modern models (SD/SDXL, MJ, 3D renderers).

---

# 2) Output Contract (keys + types)

- Return **only** valid JSON (no comments/markdown).
    
- If something doesn’t apply, use `null`.
    
- Keep text values concise (≤ 25 words).
    

```json
{
  "subject_action": {
    "subject": "string",
    "attributes": ["string"],
    "action": "string"
  },
  "style_medium": {
    "medium": "string",
    "movement_or_technique": ["string"]
  },
  "setting_era": {
    "environment": "string",
    "time_of_day_or_season": "string",
    "era_or_future": "string",
    "weather_atmosphere": "string"
  },
  "composition_camera": {
    "shot_type": "string",
    "lens_mm": "number or null",
    "aperture": "string or null",
    "dof": "string or null",
    "framing": "string"
  },
  "lighting": {
    "quality": "string",
    "direction": "string",
    "sources": ["string"]
  },
  "color_tonal_palette": {
    "harmony": "string",
    "hex": ["string"],
    "contrast": "string",
    "saturation": "string"
  },
  "mood_emotion": ["string"],
  "material_surface_detail": ["string"],
  "post_process_film_look": {
    "grade_or_stock": "string",
    "effects": ["string"]
  },
  "rendering_engine": {
    "engine": "string or null",
    "lighting_model": "string or null",
    "quality_flags": ["string"] 
  },
  "output_controls": {
    "aspect_ratio": "string",
    "resolution_px": ["number","number"],
    "cfg": "number or null",
    "steps": "number or null",
    "stylize_or_chaos": "string or null",
    "seed": "number or null",
    "sampler": "string or null",
    "upscaler": "string or null",
    "denoise_strength": "number or null",
    "hires_pass": "boolean or null"
  },
  "negative_exclusions": ["string"],
  "references_consistency": {
    "character_or_asset_id": "string or null",
    "anchors": ["string"],
    "reference_image_ids_or_links": ["string"],
    "series_note": "string or null"
  }
}
```

---

# 3) Allowed Values (curated menus)

Use **one** primary choice per category unless your brief explicitly needs more.

**Medium**  
`photo, painting, illustration, 3D render, vector, collage, woodcut, pixel art, claymation, low-poly, isometric`

**Movements/Techniques**  
`Ukiyo-e, Art Nouveau, Art Deco, Bauhaus, Impressionism, Expressionism, Surrealism, Futurism, Minimalism, Brutalism, Vaporwave, Synthwave, Solarpunk, Cyberpunk, Afrofuturism, Constructivism, Cubism, Pop Art, Graffiti, Risograph, Cyanotype, Block print, Ballpoint sketch, Ink wash, Gouache, Watercolor, Oil, Acrylic pour, Cut paper, Pressed flowers, Cross-stitch, Pixel art, Paint-by-numbers`

**Shot type**  
`macro, extreme close-up, headshot, half-body, full-body, wide, panorama, bird’s-eye, worm’s-eye, isometric, dutch angle`

**Lighting**

- quality: `soft, hard, volumetric, high-key, low-key, chiaroscuro`
    
- direction: `backlit, rim-lit, side-lit, top-lit`
    
- sources: `sun, softbox, neon, candlelight, moonlight, practical LEDs, studio`
    

**Palette**

- harmony: `monochrome, duotone, complementary, analogous, triadic, pastel, neon, grayscale, sepia, jewel tones, earth tones, iridescent, metallic`
    
- `hex`: 2–3 color codes (e.g., `["#0E6F8F","#F18F01"]`)
    
- contrast: `low, medium, high`
    
- saturation: `muted, neutral, vibrant`
    

**Mood/Emotion (pick 1–3)**  
`serene, whimsical, joyful, melancholic, nostalgic, eerie, epic, gritty, cozy, austere, determined, hopeful, solemn, triumphant, anxious, mischievous, stoic`

**Framing**  
`centered symmetry, rule of thirds, leading lines, negative space`

**Materials/Surface**  
`glossy, matte, satin, rough, weathered, patina, grain, brushstrokes, fabric weave, paper tooth, halftone, bokeh`

**Post/Film**

- grade/stock: `Portra 400, Cinestill 800T, Ilford HP5, teal-orange, neutral`
    
- effects: `vignette, bloom, halation, tilt-shift, motion blur, HDR`
    

**3D**

- engine: `Octane, Redshift, Cycles, Unreal`
    
- lighting_model: `PBR, global illumination, raytracing`
    
- quality_flags: `subsurface scattering, displacement, 8k, anisotropy`
    

---

# 4) Defaults & Auto-Fill Logic

Apply only when omitted by the brief.

- **Time of day:** choose `golden hour` (warm) or `blue hour` (cool) to match palette.
    
- **Shot:** `half-body` for characters, `wide` for environments.
    
- **Lighting:** `soft` key + `rim-lit`.
    
- **Palette:** `complementary` or `duotone` with **2–3** HEX anchors.
    
- **Photo optics:** if `medium = photo`, set `lens_mm` (85 portrait, 35 street), `aperture` (`f/2.0` portraits, `f/8` landscapes), `dof` accordingly.
    
- **Stable Diffusion/SDXL controls:** `cfg: 6–7`, `steps: 35–50`, `seed: random`.
    
- **If non-3D:** set `"rendering_engine": { "engine": null, ... }`.
    

---

# 5) Conditional Rules

- **Photo** → Fill `composition_camera.lens_mm`, `aperture`, `dof`. Consider `post_process_film_look.grade_or_stock`.
    
- **3D render** → Fill `rendering_engine` (`engine`, `lighting_model`, relevant `quality_flags`).
    
- **Vector/print** → Prefer flat colors; allow `halftone`/`misregistration`; avoid photoreal textures.
    
- **Series consistency** → Lock `output_controls.seed`, supply `references_consistency.character_or_asset_id`, and 1–2 color/prop `anchors`.
    

---

# 6) How to Brief & Generate (workflow)

1. **Write a one-sentence brief** (subject + action + setting).
    
2. **Pick one style/medium** (optionally one technique).
    
3. **Choose palette** (harmony + 2–3 HEX).
    
4. **Set lighting** (quality + direction + sources).
    
5. **Populate fields** top→bottom, letting defaults fill gaps.
    
6. **Scan for contradictions** (e.g., `overcast` + `hard shadows`).
    
7. **Add concise negatives**.
    
8. **For series**, set seed + anchors.
    

---

# 7) Quality Checklist (30-second pass)

- One clear **subject + action**
    
- Exactly **one** movement (optionally one technique)
    
- Lighting has **quality + direction + source**
    
- Palette = **one harmony + 2–3 HEX**
    
- Optics coherent with shot (lens/aperture/DOF)
    
- Output params fit subject (AR/resolution/model fields)
    
- Negatives are **short and relevant**
    
- Series fields (seed/anchors/ID) set if needed
    

---

# 8) Troubleshooting (symptom → fix)

- **Generic outputs** → Add explicit action/pose, lighting direction, and 2 HEX anchors.
    
- **Style soup** → Keep one movement; at most one technique.
    
- **Muddy color** → Use `complementary` or `duotone`, `contrast: high`, enforce 2–3 HEX.
    
- **Flat lighting** → Use `side-lit` or `backlit` + `rim-lit`; `dof: shallow` (f/2–f/2.8).
    
- **Anatomy issues** → Reduce style stack, `cfg: 5–7`, negatives: `"no extra fingers"`, add `"anatomically correct"`.
    
- **Plastic CGI (unwanted)** → Add `subsurface scattering`, `roughness variation`, `film grain`; enable `global illumination` or `raytracing`.
    
- **Busy frame** → Enforce `rule of thirds` or `centered symmetry`; simplify palette to two hues; add `negative space`.
    
- **Series drift** → Lock `seed`, repeat `character_or_asset_id`, keep 1–2 anchors, vary one variable per iteration.
    

---

# 9) Model Integration Notes

- **Midjourney**: use `aspect_ratio` and `stylize_or_chaos`; MJ ignores `cfg/steps`. Keep them but set as `null` if you’re exporting 1:1 to MJ.
    
- **Stable Diffusion / SDXL**: use `cfg`, `steps`, `sampler` (e.g., `DPM++ 2M Karras`), optional `hires_pass`, `upscaler`.
    
- **3D (Octane/Redshift/Cycles/Unreal)**: fill `rendering_engine` and give material/lighting flags; the rest still guides look dev.
    

---

# 10) Example A — Photoreal Character (JSON)

```json
{
  "subject_action": {
    "subject": "female astronaut",
    "attributes": ["late-20s", "matte carbon suit with orange wrist tag"],
    "action": "adjusting helmet chin strap"
  },
  "style_medium": {
    "medium": "photo",
    "movement_or_technique": ["retro-futurist minimalism"]
  },
  "setting_era": {
    "environment": "windswept salt flat horizon",
    "time_of_day_or_season": "blue hour",
    "era_or_future": "near-future 2040s",
    "weather_atmosphere": "dust haze"
  },
  "composition_camera": {
    "shot_type": "half-body",
    "lens_mm": 85,
    "aperture": "f/2.0",
    "dof": "shallow",
    "framing": "centered symmetry"
  },
  "lighting": {
    "quality": "soft",
    "direction": "backlit",
    "sources": ["low sun", "practical suit LEDs", "rim-lit"]
  },
  "color_tonal_palette": {
    "harmony": "complementary",
    "hex": ["#0E6F8F", "#F18F01"],
    "contrast": "high",
    "saturation": "neutral"
  },
  "mood_emotion": ["determined", "quiet awe"],
  "material_surface_detail": ["matte carbon fiber", "scuffed visor micro-scratches", "fine film grain"],
  "post_process_film_look": {
    "grade_or_stock": "Portra 400",
    "effects": ["subtle bloom", "vignette"]
  },
  "rendering_engine": {
    "engine": null,
    "lighting_model": null,
    "quality_flags": []
  },
  "output_controls": {
    "aspect_ratio": "3:2",
    "resolution_px": [1536, 1024],
    "cfg": 6,
    "steps": 40,
    "stylize_or_chaos": "low",
    "seed": 1234,
    "sampler": null,
    "upscaler": null,
    "denoise_strength": null,
    "hires_pass": null
  },
  "negative_exclusions": ["no text overlays", "no watermarks", "no extra fingers", "no color banding", "no low contrast"],
  "references_consistency": {
    "character_or_asset_id": "Astra-01",
    "anchors": ["orange wrist tag", "teal visor tint"],
    "reference_image_ids_or_links": [],
    "series_note": "keep suit geometry and visor tint stable"
  }
}
```

---

# 11) Example B — Vector/Print Environment (JSON)

```json
{
  "subject_action": {
    "subject": "isometric city block",
    "attributes": ["clean geometry", "Art Deco motifs"],
    "action": "night market bustle implied by light pools"
  },
  "style_medium": {
    "medium": "vector",
    "movement_or_technique": ["Art Deco", "Risograph"]
  },
  "setting_era": {
    "environment": "neon market street",
    "time_of_day_or_season": "night",
    "era_or_future": "contemporary",
    "weather_atmosphere": "light rain"
  },
  "composition_camera": {
    "shot_type": "isometric",
    "lens_mm": null,
    "aperture": null,
    "dof": null,
    "framing": "negative space"
  },
  "lighting": {
    "quality": "hard",
    "direction": "side-lit",
    "sources": ["neon signage", "shop windows"]
  },
  "color_tonal_palette": {
    "harmony": "duotone",
    "hex": ["#FF2AA1", "#00B0FF"],
    "contrast": "medium",
    "saturation": "vibrant"
  },
  "mood_emotion": ["whimsical", "lively"],
  "material_surface_detail": ["flat fills", "halftone grain", "print misregistration"],
  "post_process_film_look": {
    "grade_or_stock": "print-like",
    "effects": ["subtle halftone", "tiny misregistration"]
  },
  "rendering_engine": {
    "engine": null,
    "lighting_model": null,
    "quality_flags": []
  },
  "output_controls": {
    "aspect_ratio": "1:1",
    "resolution_px": [1024, 1024],
    "cfg": null,
    "steps": null,
    "stylize_or_chaos": null,
    "seed": null,
    "sampler": null,
    "upscaler": null,
    "denoise_strength": null,
    "hires_pass": null
  },
  "negative_exclusions": ["no gradients", "no photoreal textures", "no watermarks"],
  "references_consistency": {
    "character_or_asset_id": null,
    "anchors": ["magenta-cyan duotone"],
    "reference_image_ids_or_links": [],
    "series_note": "keep grid spacing and sign geometry consistent"
  }
}
```

---

## Final Notes

- Keep it **single-style, single-palette** unless you have a deliberate reason to blend.
    
- The **three biggest levers** are: **lighting** (quality/direction/source), **palette** (harmony + HEX), and **optics** (shot/lens/aperture/DOF).
    
- For series, **lock seed + anchors** and change one variable per iteration.