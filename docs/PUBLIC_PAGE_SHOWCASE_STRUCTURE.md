# Tiger Studio Public Page Structure

This document defines the public GitHub Pages structure for Tiger Studio.
It keeps the page visually driven, video-editor-first, and public-safe.

Korean note:
Tiger Studio 공개 페이지는 단순 캡처 앱 소개가 아니라, 영상편집 중심의 크리에이터 스튜디오 쇼케이스로 보여야 합니다.

## Product Position

Main name:
Tiger Studio

Secondary name:
Repository continuity only: the public URL may contain `tigercapture`, but visible product copy uses Tiger Studio.

Primary positioning:
Subculture-ready video editor for screen, shorts, and character creators.

Korean support copy:
화면녹화, 쇼츠, 캐릭터 영상을 한 곳에서 만드는 영상편집 스튜디오.

## Public Safety Rules

- Do not expose non-release materials, unpublished branches, internal tool notes, or private build details.
- Public repo content should stay limited to the landing page, public docs, release notes, installers, screenshots, catalog images, and release-safe specs.
- Keep English as the main public copy. Use Korean as supporting copy, not as the only explanation.
- Present Tiger Studio as video-editor-first. Screen capture is one workflow, not the product identity.
- Keep `TigerCapture` out of visible product copy. `tigercapture` may appear only in repository URLs or technical continuity text.

## Visual Direction

Use a game-studio style product showcase:

- Full-screen hero.
- Large background image or product screenshot.
- Sparse text over visual media.
- Fixed slim navigation.
- Section-by-section scroll scenes.
- One dominant visual per section.
- Small right-side step list or scene index.
- Current scroll scene updates both the large image and the layered cinematic backdrop.
- Feature cards should be secondary; the first impression must be visual.

Avoid:

- Dense feature grids as the main experience.
- Long developer explanations.
- Tiny screenshots.
- A page that reads as a capture utility.
- Old TigerCapture-branded hero artwork as the first signal.

## Page Order

1. Top Navigation
2. Full-screen Hero
3. What You Can Make
4. Character Commentary Output
5. Product Spec
6. Positioning
7. Release Honesty
8. Product Walkthrough
9. Footer

## 1. Top Navigation

Purpose:
Give the page a polished studio/product-site feeling without making it heavy.

Recommended labels:

- Tiger Studio
- Make
- Showcase
- Spec
- Download

Behavior:

- Fixed on desktop.
- Compact on mobile.
- Link `Download` to the latest public installer release when downloads are
  open. While downloads are paused, link it to the local `Not yet` download
  notice.
- Link `Spec` to the public product spec Markdown.

## 2. Full-screen Hero

Purpose:
Make the product name and product category immediately clear.

Visual:
Use a large timeline/editor screenshot as the main background.
Layer a character/actor-related image subtly on top or to the side when possible.

H1:
Tiger Studio

Subtitle:
Subculture-ready video editor for screen, shorts, and character creators.

Support line:
Local-first creator video studio for Windows.

Korean subcopy:
화면녹화, 쇼츠 편집, Live2D/Spine/MMD/VRM 캐릭터, 음성, 음악, 발표 페이지를 한 프로젝트에서 다루는 로컬 우선 영상편집 스튜디오입니다.

CTA:

- Download installer, or `Download: Not yet` while downloads are paused
- View public spec

Workflow pills:

- Timeline editor
- Screen polish
- Character actors
- Voice / Music
- AR / PBR

Design rules:

- H1 must be the largest text on the page.
- The first viewport must show `Tiger Studio`, the short positioning line, and the download button.
- Do not put the hero text inside a card.
- Do not show `TigerCapture` as a product name.

## 3. What You Can Make

Purpose:
Show outcomes, not just features.

Layout:
Use four large vertical visual tiles. Each tile uses a product catalog image as its background.

Tile 01:
Polished screen recordings

Copy:
Screen Studio-style cursor, zoom, click, hotkey, and export polish for tutorials and product videos.

Image:
`docs/product_catalog/slides_en/06_timeline.png`

Tile 02:
Character videos

Copy:
Live2D, Spine, MMD, and VRM actor tracks for edited videos, shorts, and avatar-driven scenes.

Image:
`docs/product_catalog/slides_en/17_live2d_spine.png`

Tile 03:
Shorts and social clips

Copy:
Captions, vertical templates, hooks, publish packages, and render queue handoff for creator workflows.

Image:
`docs/product_catalog/slides_en/21_creator_assist.png`

Tile 04:
Voice, music, and presentation videos

Copy:
Voice Lab direction, Music Lab, subtitles, and PPT-style pages for explainer and character content.

Image:
`docs/product_catalog/slides_en/14_music_lab.png`

Design rules:

- Tiles should feel like product scenes, not small cards.
- Text should sit over a dark gradient at the bottom.
- The image must remain the main signal.

## 4. Character Commentary Output

Purpose:
Show one finished character-video result after the user understands the output
categories and before the product spec cards.

Recommended title:
Character Commentary Output

Recommended headline:
A finished Live2D voice scene.

Copy:
A 30-second Tokyo night-view commentary scene with Japanese TTS, subtitles,
Live2D motion, natural blink, and lip-sync.

Behavior:

- Do not autoplay this video. The AI editing process demo already provides the
  moving first proof; this section is a user-played output sample.
- Use `controls`, `playsinline`, `preload="metadata"`, and a poster image.
- Keep the file compressed for GitHub Pages. Prefer a 540p/720p web demo asset
  instead of the local high-bitrate proof.
- Place this section between What You Can Make and Product Spec.

Design rules:

- Treat it as a finished result, not another process demo.
- The video can be large, but the copy should stay short.
- On mobile, keep it single-column and avoid auto playback.

## 5. Product Spec

Purpose:
Give users a fast map of product areas after they understand what the app can make.

Cards:

- Timeline Video Editor
- Screen Recording Polish
- Character Actors
- Voice Lab and Subtitles
- Music Lab and Audio
- PPT / Presentation Pages
- AR / PBR / 3D Compositing
- AI Actions and Automation

Design rules:

- Keep titles short.
- Keep text factual.
- This section can be card-based because it is secondary information.

## 6. Positioning

Purpose:
Prevent unrealistic comparisons while still making the product direction clear.

English copy:
Tiger Studio is not trying to replace DaVinci Resolve, CapCut, OBS, Live2D Cubism, or VTube Studio directly. It brings the creator-facing parts together into one local editing workflow.

Korean copy:
Resolve급 전문 후반작업 툴이나 Cubism 같은 모델 제작툴을 대체하는 것이 아니라, 캐릭터와 화면녹화, 쇼츠, 음성, 음악을 하나의 영상편집 흐름으로 묶는 것이 핵심입니다.

Design rules:

- Keep this section quiet and credible.
- Use it as a trust section, not as a hype block.

## 7. Release Honesty

Purpose:
Make public claims credible and measured.

Rows:

- Final Product Readiness: 99/100
  Release claims are still gated by real broadcast platform evidence.

- CapCut-style workflow: 89.38/100
  Shorts planning and creator workflow coverage are strong; cloud/mobile collaboration remains a gap.

- Descript-lite workflow: 88/100
  Scoped AI script edit value is claim-ready within reviewed safe-apply boundaries.

- NLE readiness: 91/100
  Not a Premiere/Resolve-class professional NLE claim.

- Character Asset Hub
  Local corpus scanning supports Live2D and Spine assets strongly, with VRM/MMD workflows tracked separately.

- Voice Lab direction
  Style-Bert-VITS2 sidecar direction exists, but server/runtime readiness is described as sidecar-dependent.

Design rules:

- This section should be readable and restrained.
- Avoid turning readiness scores into marketing guarantees.

## 8. Product Walkthrough

Purpose:
This is the main visual catalog. It should feel like a scrolling studio showcase.

Layout:

- Left side: very large sticky image preview.
- Right side: small vertical scene index.
- Current scene changes the preview image.
- Current scene also changes the section backdrop image.
- The backdrop should be layered, not a single flat blur:
  - a deep, oversized color-wash layer for atmosphere,
  - a shallow, low-opacity detail layer so the current slide shape remains readable,
  - a dark matte/gradient layer to protect foreground text,
  - a subtle grain or scanline texture to avoid a cheap glass-panel look.
- The right-side item should be compact. It is a navigator, not the main content.

Scene list:

| No. | Title | Image | Public Message |
| --- | --- | --- | --- |
| 01 | Multi-Environment Editing Studio | `docs/product_catalog/slides_en/01_studio_overview.png` | The same project can spread across preview, timeline, actors, 3D, nodes, and audio displays. |
| 02 | Studio Surface | `docs/product_catalog/slides_en/02_studio_surface.png` | The editor surface: preview, timeline, media pool, workbench, and contextual controls. |
| 03 | AI Workflow | `docs/product_catalog/slides_en/03_ai_workflow.png` | Reviewable AI planning and structured actions instead of hidden one-shot mutations. |
| 04 | PPT Maker | `docs/product_catalog/slides_en/04_ppt_maker.png` | Timeline-native presentation pages with editable media, typography, and export paths. |
| 05 | Media Pool | `docs/product_catalog/slides_en/05_media_pool.png` | Import, organize, inspect, and prepare project media before dropping it into the timeline. |
| 06 | Timeline | `docs/product_catalog/slides_en/06_timeline.png` | Clip editing, tracks, timing, thumbnails, frame repair, and story structure in one place. |
| 07 | Effects | `docs/product_catalog/slides_en/07_effects.png` | Effect presets and clip processing that stay connected to preview/export parity checks. |
| 08 | Transitions | `docs/product_catalog/slides_en/08_transitions.png` | Timeline transitions and creator-style motion pieces for faster edit assembly. |
| 09 | Typography | `docs/product_catalog/slides_en/09_typography.png` | Captions, titles, layout, and text animation as editable production elements. |
| 10 | Keyframes | `docs/product_catalog/slides_en/10_keyframes.png` | Motion, timing, and parameter animation for precise creator edits. |
| 11 | Color | `docs/product_catalog/slides_en/11_color.png` | LUTs, scopes, color metadata, and workflow checks for repeatable output. |
| 12 | Node Graph | `docs/product_catalog/slides_en/12_node_graph.png` | A workbench surface for graph-based effects and compositing experiments. |
| 13 | Node Effects | `docs/product_catalog/slides_en/13_node_effects.png` | Effect nodes, masks, and previewable processing chains for advanced edits. |
| 14 | Music Lab | `docs/product_catalog/slides_en/14_music_lab.png` | Prompt-driven composition creates editable sections, chords, MIDI notes, and renderable stems. |
| 15 | Audio Workbench | `docs/product_catalog/slides_en/15_audio_workbench.png` | Sound Editor, mix controls, loudness helpers, and production audio surfaces. |
| 16 | Audio Curves | `docs/product_catalog/slides_en/16_audio_curves.png` | Curves, automation, dynamics, EQ, and diagnostics for shaping sound over time. |
| 17 | Live2D / Spine | `docs/product_catalog/slides_en/17_live2d_spine.png` | Character actors as timeline assets, with compatibility and render diagnostics. |
| 18 | VRM | `docs/product_catalog/slides_en/18_vrm.png` | VTuber avatar workflows, performance-source mapping, and broadcast output foundations. |
| 19 | MMD | `docs/product_catalog/slides_en/19_mmd.png` | PMX/PMD and VMD-oriented actor workflows for local character production. |
| 20 | AR / PBR | `docs/product_catalog/slides_en/20_ar_pbr.png` | 3D object compositing, material controls, depth-aware placement, and render parity targets. |
| 21 | Creator Assist | `docs/product_catalog/slides_en/21_creator_assist.png` | Short-form planning, caption beats, publish variants, and safe apply workflows. |
| 22 | Export | `docs/product_catalog/slides_en/22_export.png` | Render queue, delivery presets, diagnostics, and export readiness checks. |
| 23 | Specification Index | `docs/product_catalog/slides_en/23_closing.png` | The catalog closes with a compact release-safe map of the current product surface. |

Design rules:

- The preview image should be at least four times wider than the scene index on desktop.
- The scene index should feel like a control rail.
- The current scene backdrop should feel cinematic: blurred, darkened, and still lightly recognizable behind the content.
- On mobile, collapse to single-column: full-width preview first, then compact scene blocks.
- On mobile, the Product Walkthrough preview must fit inside the phone viewport with no horizontal scroll.
- Do not constrain the Product Walkthrough preview to a narrow card; use the available viewport width, but never exceed it.

## 9. Footer

Purpose:
Give release continuity without distracting from the product page.

Recommended copy:
Public distribution page for Tiger Studio.

Optional:
Installer SHA-256 for the current public installer, or a clear `Not yet`
download notice while downloads are paused.

Design rules:

- Keep the footer small.
- Do not add internal repository or build-process details.

## Update Checklist

Before publishing a public page update:

- The first viewport clearly says `Tiger Studio`.
- `TigerCapture` does not appear as visible product copy; `tigercapture` may remain only in repository URLs or technical continuity notes.
- The page reads as a creator video editor, not a capture app.
- All images are local public assets or stable public release assets.
- No non-release packages, private build notes, or internal workflow details are exposed.
- Image links are valid.
- Mobile first viewport shows product name, one-line explanation, and the download button.
- Scroll scenes update preview and background together.
