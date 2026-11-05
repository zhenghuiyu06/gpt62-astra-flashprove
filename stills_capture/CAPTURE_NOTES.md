# CAPTURE_NOTES — GPT-6.2 Astra episode gaps

Captured 2026-11-05. Browser viewport 1920×1113. No login. PNG unless noted. Nothing below was drawn or relabeled; chart numbers are only what the live page showed.

Cookie / overlays: OpenAI article had no consent banner. Dropday “Your privacy, your choice” was dismissed with **Reject optional** before shooting. Anthropic and GitHub had no banner. The Verge privacy bar stayed (close control had no accessible name); it covers the byline strip only.

## 1. OpenAI — accelerating engineering for the physical world

URL: https://openai.com/index/accelerating-engineering-for-the-physical-world/
Status: **loaded (HTTP page, not 403)**. No captcha.

There is **no inline device/PCB photo gallery**. The only image link in the article is the enclosure drawing. PCB is prose under “Electrical design.” Device appearance is the hero video poster (purple Codex talk device).

### BenchCAD — read this before captioning

- Paragraph in `S02_openai_measuring_progress_0875.png` (verbatim on screen): a newer **internal** model average score **0.875**, compared with **0.594** for **GPT-6 Astra** at its highest reasoning setting. BenchCAD 2.0 = reconstruct 3D parts/assemblies and identify circuit-board connections.
- Chart (`S02_openai_benchcad_chart.png`) title: **“Performance of GPT-6 Astra and our Internal Model on BenchCAD 2.0.”** Legend: GPT-6 Astra and Internal Model. Y-axis “Mean BenchCAD 2.0 score” ticks 0, 0.2, 0.4, 0.6, 0.8, 1. X-axis “Relative cost proxy (log scale)” with **no numeric x labels**. **The chart does not print 0.875 or 0.594.** Do not caption 0.875 as GPT-6.2 Astra. The upper series is labeled Internal Model.

| File | Where | What |
| --- | --- | --- |
| `S13_openai_article_hero.png` | `06_OpenAI_Hardware/stills/` | Hero: 2026-11-03, title, video poster of the purple device. 1920×1113. |
| `S14_openai_device_section_text.png` | same | “Designing a device with Astra” plus enclosure / PCB / UI bullets. 1920×1113. |
| `S14_openai_device_bullets_and_codex_chart_start.png` | same | Rest of device bullets, manufacturing-gap paragraph, start of Codex-usage chart. 1920×1113. |
| `S14_openai_codex_usage_chart.png` | same | Full chart “Median daily Codex use across OpenAI hardware teams,” endpoint labeled 212M. 1377×517. |
| `S14_openai_enclosure_diagram.png` | same | **Original file** from the article’s “enclosure” link (`prototype-device-enclosure-diagram.png` on images.ctfassets.net), not a redraw. Sheet “01 / SEAT RIM & WINDOW”, “ENCLOSURE 04 - BODY-CENTRED”, title block “09 / Black bezel”, Owner OpenAI. 7017×4963. |
| `S14_openai_enclosure_diagram_viewport.png` | same | Browser view of that same PNG (window-fit, bottom of the sheet slightly cropped). 1920×1113. |
| `S02_openai_benchcad_chart.png` | `06_…` **and** `02_BenchCAD/stills/` | Chart element only. 677×517. |
| `S02_openai_benchcad_chart_wide.png` | both | Same chart with page margin. 1377×517. |
| `S02_openai_measuring_progress_0875.png` | both | “Measuring progress…” paragraph with **0.875 / 0.594** plus the chart. 1920×1113. |
| `S16_openai_cgr_section.png` | `06_OpenAI_Hardware/stills/` | “Safely deploying…” + Chip Ganassi Racing paragraphs + start of Ortman quote. 1920×1113. |
| `S16_openai_cgr_mazda.png` | `06_…` only | Matthew Ortman (CGR) quote, Mazda research announcement, “Front car aerodynamics” video frame. 1920×1113. |
| `S16_openai_mazda_nose.png` | `06_…` | “Exploring nose designs” frame (Original) + Mazda caption (agreement for use obtained from Mazda; republication prohibited). 1920×1113. |
| `S16_openai_mazda_quote.png` | `06_…` | Nose-variant labels (Original, Broad crown, Long recovery, Lower central crown, Refined recovery), Akihiro Nakata (Mazda) quote, “Help shape AI…” close. 1920×1113. |

Misses on this URL: no separate PCB photograph and no multi-image device gallery to shoot. Not a block.

## 2. Dropday — game screenshot SVGs

URL: https://dropday.ai/c/game-screenshot-svgs
Status: **loaded** after dismissing the privacy dialog. Credit UI and inferred-credit warning are on the page.

Visible credit conflict (do not upgrade to verified GPT-6.2):

- Details **BUILT WITH: GPT-6 Astra** (pill), attributed to @FixlationAI.
- Timeline quote: “INSANE SVG's from GPT 6.2 Astra!…”
- Models-reasoning tooltip (opened via the Models info control): creator credit stays GPT-6 Astra; “source says ‘INSANE SVG's from GPT 6.2 Astra!’; post says ‘GPT-6.2 Astra’.”
- Warning under Description: “Descriptions, tags, and model credits may be AI-generated or inferred from public sources and can be incomplete or wrong.”

| File | What |
| --- | --- |
| `04_Game_SVG/stills/S09_dropday_hero.png` | Title + Minecraft video poster. 1920×1113. |
| `S09_dropday_built_with_credit.png` | How-it-grew 6.2 quote **and** Built with GPT-6 Astra sidebar; warning at the bottom edge. 1920×1113. |
| `S09_dropday_built_with_crop.png` | Tight crop: @FixlationAI, BUILT WITH GPT-6 Astra, tags. 700×420. Warning not in this crop. |
| `S09_dropday_inferred_warning.png` | Warning sentence readable, plus Built with pill and Minecraft challenge row. 1920×1113. Header slightly blurred. |
| `S09_dropday_models_reasoning.png` | Tooltip with the 6.2-vs-Astra wording, Built with pill, warning. 1920×1113. |
| `S09_dropday_minecraft_gallery.png` | Minecraft challenge strip (Opus 5.5 and GPT-6 Astra thumbs, Sep 2026) + warning. 1920×1113. |
| `S09_dropday_similar_games.png` | Same strip plus Similar: GPT-5.6 Pro Minecraft Clone, Minecraft \| Blender World. 1920×1113. |

## 3. Anthropic — provable inference

URL: https://www.anthropic.com/research/provable-inference
Status: **loaded**. Published Nov 20, 2026, Frontier Red Team. Title “Progress on provable inference for large language models.”

Numbers read off the page (not invented):

- Executive summary: Llama 4 Maverick, 400B MoE, one H100, about **110 tokens/second**, proof size **~19 MB** per 1,024-token request, 4-bit weights, ~70–95× the GPU time of vLLM.
- Evaluation: offline phase ~39 minutes; online batch of 24 requests **223 seconds**, **110 tokens per second**, each proof **18.78 MB**.
- Prior work: **VerInf** reports 14.3 hours for 1,000 tokens on a DGX Spark, **93.6 GB** proof; FlashProve same model **110 tokens/second** on one H100, **19 MB** proofs verifiable in seconds.

| File | What |
| --- | --- |
| `08_FlashProve/stills/S21_anthropic_provable_inference_hero.png` | Hero title, chain illustration, date, TOC. 1920×1113. |
| `S24_anthropic_flashprove_110tps_19mb.png` | Executive summary with 110 tok/s and ~19 MB. 1920×1113. |
| `S24_anthropic_evaluation_numbers.png` | Guarantees (19 MB / 232 GB weights) + Evaluation 18.78 MB / 110 tok/s. 1920×1113. |
| `S24_anthropic_verifier_engineering.png` | Verifier timing vs vLLM and “Engineering the system.” 1920×1113. |
| `S24_anthropic_prior_work.png` | Prior-work open (zkML history). 1920×1113. |
| `S24_anthropic_verinf_93gb_vs_19mb.png` | VerInf 93.6 GB vs FlashProve 19 MB / 110 tok/s paragraph. 1920×1113. |

## 4. GitHub — anthropics/FlashProve

URL: https://github.com/anthropics/FlashProve
Status: **loaded**, public, no login. About: “A research prototype for zero-knowledge proofs of AI inference. Not maintained.” Repo file list includes a `lean` directory.

Lean: https://github.com/anthropics/FlashProve/tree/main/lean (folders Alg, Ask, VerifiableInference, ZKCP, … plus THEOREM.md, STATEMENTS.html, CHECKING.md).
Theorem: https://github.com/anthropics/FlashProve/blob/main/lean/THEOREM.md (1411 lines). Heading on screen: “What is proved in Lean: the six theorems, and the soundness theorem on verify beneath sound.” Soundness bound on screen: about q/2^124 + 2^-101.

| File | What |
| --- | --- |
| `08_FlashProve/stills/S22_flashprove_github_repo_header.png` | Repo header + file tree including `lean`. 1920×1113. |
| `S22_flashprove_github_readme.png` | README: What it is / What model it runs (110 tok/s) / What is proved (Lean 4, link to lean/THEOREM.md). 1920×1113. |
| `S22_flashprove_github_readme_proved.png` | Continuation: agent instructions + hardware/software table. 1920×1113. |
| `S25_flashprove_lean_folder.png` | `lean/` directory listing (top of tree). 1920×1113. |
| `S25_flashprove_lean_theorem.png` | THEOREM.md top, six theorems, sidebar shows THEOREM.md selected. 1920×1113. |
| `S25_flashprove_lean_theorem_continued.png` | Rest of the theorem list and “The Lean verifier.” 1920×1113. |

Did not open every Lean submodule (deep dive not required). STATEMENTS.html not screenshotted.

## 5. ChatGPT Images 2.6 — saved-reference @ mention

Status: **MISSING — needs a signed-in ChatGPT account.**

- https://openai.com/index/introducing-images-2-6/ loaded. Full visible article text (~8.3k chars) has **no** “saved reference”, “@”, “mention”, or “reference photo”.
- https://help.openai.com/en/search?q=images%202.6%20saved%20reference returned “UH OH. THAT PAGE DOESN'T EXIST.” Not a captcha.
- No product UI was opened. Do not fake an @-mention chip.

Optional Verge hero (not the @ UI): `07_ChatGPT_Images_2_6/stills/S17_verge_images26_gifs_hero.png` — https://www.theverge.com/ai-artificial-intelligence/1026474/openai-chatgpt-animated-gifs-images-2-6 — headline “ChatGPT will now make you animated GIFs”, Nov 4, 2026, Emma Roth, OpenAI-knot illustration. Privacy bar still covers the lower byline. 1920×1113.

## Failures

- OpenAI article was **not** blocked this run (earlier curl 403 does not apply to this browser session).
- No BenchCAD digits were added to the chart image.
- Images 2.6 saved-reference @ mention: not on the public article; account UI not attempted.
