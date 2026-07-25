# Tiger Studio Public Product Spec

This document is the release-safe public specification for Tiger Studio.
The public repository URL may retain `tigercapture` for distribution
continuity, but the visible product name is Tiger Studio.

## Status Labels

- **Available**: implemented in the current source and exposed through a user
  interface, an Action surface, or both.
- **Conditional**: implemented, but requires an optional local model, external
  sidecar, provider, host application, or compatible asset.
- **Limited / Experimental**: usable for its stated scope, but not a parity
  claim against a specialized professional application.
- **Planned**: product direction only. Planned items are not presented as
  current product capability.

## Product Position

Tiger Studio is a local-first Windows video editor for screen, short-form, and
character-driven media. The main timeline connects focused creation rooms for
motion graphics, painting, music, voice, presentations, character performance,
broadcast output, and AR/PBR compositing.

Tiger Studio is designed so a creator or an AI assistant can work on editable
project data instead of returning only disconnected generated files.

## Product Shell and Media Workflow

### Studio and Capture

**Available**

- Tiger Studio provides the full editing workspace.
- The lightweight Capture application remains a separate surface for screen
  recording and capture-to-Studio handoff.
- Screen-recording polish includes cursor sidecars, cursor smoothing, click and
  drag feedback, hotkey badges, zoom planning, framing, shadows, and vertical
  layout handling.
- Startup, loading, empty, progress, and failure states use product-facing
  feedback instead of relying on debug output.

The Capture launcher and Tiger Studio are related workflows, but they are not
presented as one undifferentiated window.

### Media Pool and Intake

**Available**

- Media Pool intake covers video, audio, still images, typography assets,
  actor assets, and supported 3D formats.
- Video and media assets can be dragged from Media Pool into timeline tracks.
- 3D files are classified before opening the AR/PBR preview path.
- Timeline clips, current video frames, typography, video, audio, and 3D assets
  can also be passed into focused tools such as PPT Maker.
- Media relink and missing-asset diagnostics support moved project media.

**Conditional / Limited**

- YouTube intake depends on the configured downloader path and source
  availability.
- FBX is accepted as an import source, but support is limited compared with
  glTF/GLB/VRM and may require conversion or material repair.

## Timeline Video Editor

### Timeline and Clip Editing

**Available**

- Multi-track video, audio, typography, effect, transition, actor, 3D, and
  presentation-oriented timeline data.
- Clip placement, move, trim, split, duplicate, delete, ripple-oriented edits,
  track targeting, selection, snapping, markers, In/Out ranges, and auditions.
- Thumbnail strips, clip-state badges, grade/effect overlays, waveform lanes,
  and playhead-focused visual treatment.
- Drag-and-drop is the preferred path for placing media and actors.
- Structured project save/load preserves editor, music, actor, and tool state.

### NLE-Oriented Workflows

**Available / Limited**

- Project bins, source records, source monitoring, storyline helpers, multicam
  structures, audition takes, markers, and readiness diagnostics are exposed
  through focused NLE modules and Actions.
- Proxy and preview-acceleration helpers exist for demanding media.
- These tools improve creator editing workflows but do not constitute a
  Premiere Pro or DaVinci Resolve parity claim.

### Preview, Export, and Delivery

**Available**

- Main preview and pop-out preview surfaces.
- H.264/MP4-oriented export paths, render queue, batch export helpers, and
  export progress/cancellation surfaces.
- Preview/export parity checks for effects, overlays, color, actors, and AR/PBR
  composites.
- Project health, media audit, crash-recovery, autosave/recovery where
  supported by the focused tool, and release-readiness QA.

## Editing and Finishing Tools

### Effects, Transitions, and Screen Polish

**Available**

- Clip effects, transitions, filters, sharpen, vignette, chromatic aberration,
  chroma key, background removal helpers, stabilization, picture-in-picture,
  zoom actors, and creator presets.
- GPU preview paths are used where compatible; CPU fallbacks remain for
  unsupported or ordering-sensitive effects.
- Comparison templates support original/current, effects off/on, color off/on,
  and multi-variant review states.

### Color, VFX, Masks, and Nodes

**Available**

- Color grading controls, scopes, LUT/management helpers, before/after review,
  and clip/track grade state.
- Node-style effect workflows, adjustment behavior, masks, rotoscope-oriented
  editing, chroma-key masks, and object-tracking integration.
- Preview/export checks verify that processing is visible in encoded output.

**Limited**

- This is a creator finishing workflow, not a full Resolve/Fusion color and VFX
  parity claim.
- HDR/OCIO and advanced interchange claims remain gated by measured
  preview/export parity.

### Typography, Subtitles, and Overlays

**Available**

- Editable typography, subtitle tracks, text overlays, styles, animation
  presets, timing, and export rendering.
- Subtitle data can drive Voice Lab generation and actor lip-sync workflows.
- Typography assets can be dragged into PPT Maker and other compatible
  creation surfaces.

## Focused Creation Rooms

### Motion Designer

**Available**

- Independent motion-composition documents with layers, keyframes, curves,
  parenting, masks, adjustment layers, alpha/luma track mattes, blend modes,
  behaviors, effects, and deterministic rendering.
- Shape paths, trim paths, vector repeaters, text animation by character, word,
  or line, and editable cut-paper rigs.
- Generic layer replicators, movement-derived motion blur, impact behavior,
  directional blur, displacement, corner pin, mesh warp, and paper fold.
- Explicit 2.5D camera projection, layer depth, parallax, and camera exclusion
  for ordinary 2D layers.
- Editable paper-paste composites with contact shadows, tape, and staples.
- Advanced presets for headline slams, paper reveals, cutout collage, camera
  pushes, and beat-oriented montage.
- Structured `motion.*` Actions, prompt/reference generation planning,
  validation, templates, plugin-management foundations, and MP4 export.

**Public evidence**

- The public Editorial Motion Graphics demo is a real 10-second, 1280x720,
  30fps render using isolated subject layers, animated paper fragments, track
  mattes, 2.5D depth, motion blur, and impact timing.

**Limited**

- The 2.5D camera is an editorial layer projection system, not a complete 3D
  scene graph or After Effects parity claim.
- Native AE project interchange, arbitrary third-party effect hosting, and
  complete expression compatibility are not claimed.

### Painter

**Available**

- Standalone canvas with editable brush strokes, layers, selection, transforms,
  undo/redo, image intake, and output.
- Structured paint Actions allow AI-assisted brush and layer operations while
  keeping the result in the Painter document workflow.
- The public moonlit-painting process video uses real Tiger Studio Painter
  actions, editable generated layers, measured refinement, and UI evidence.

**Limited**

- Painter is a creator paint room, not a Photoshop, Krita, or full raster
  production-suite parity claim.

### PPT Maker

**Available**

- Independent timeline-native presentation editor with slide thumbnails,
  canvas, inspector, media pool, document tools, tables, editable chart data,
  formulas, shapes, text, images, video, and actor placeholders.
- Built-in templates for common title, body, comparison, report, media hero,
  3D showcase, timeline recap, and typography layouts.
- Drag-and-drop intake from editor media, timeline clips, typography, images,
  video, audio, AR/PBR, VRM, and MMD sources.
- Element animation for appear, fade, move, and scale with editable timing
  lanes and click sequence metadata.
- Undo/redo, autosave/recovery, project files, validation, and structured
  `ppt.*` Actions.
- Export to editable PPTX, PDF through an available office backend, and H.264
  MP4 with basic cut/fade transitions and optional audio.
- Best-effort PPTX import for text boxes, tables, pictures, and simple shapes.
- Native editable PowerPoint chart output for supported chart data.

**Conditional / Limited**

- PDF conversion requires LibreOffice or PowerPoint COM.
- PPTX import does not preserve every master, SmartArt object, advanced chart,
  embedded medium, animation, or theme inheritance rule.
- MP4 export does not claim full PowerPoint animation/transition parity.

### Sound Editor

**Available**

- Audio tracks, clips, waveform views, transport, gain/pan, fades, effects,
  automation, buses, loudness helpers, dialogue cleanup controls, and mix
  diagnostics.
- Audio extraction and separation/provider boundaries are exposed where the
  configured backend is available.
- Generated music and voice files enter the same audio-track workflow.

### Composer and Music Lab

**Available**

- Prompt-to-composition planning for genre, mood, BPM, key, sections, chords,
  tracks, and note data.
- Editable arranger blocks, section regeneration/resizing, note operations,
  MIDI export, rendered preview, stems, timeline placement, and initial
  auto-balance.
- Sample/SoundFont production is the default user-facing route with a studio
  master and articulation/expression safety profile.
- Orchestral and genre-specific planners can produce larger structured
  arrangements than the basic nine-role layout.
- Structured `music.*`, `midi.*`, and `audio.*` Actions.

**Conditional / Limited**

- Advanced AI or external production renderers must be selected and configured
  explicitly.
- Music Lab is not a full DAW, piano-roll workstation, VST host, vocal
  generator, or replacement for dedicated orchestration software.

### Voice Lab

**Available**

- Visible voice-provider catalog with readiness and installation guidance.
- Subtitle-to-speech planning and synthesis into durable generated WAV files.
- Generated dialogue can be placed on aligned timeline audio tracks.
- TTS timing can drive Live2D mouth, blink, placement, and dialogue motion.
- Higher-level dialogue-take Actions can create subtitles, voice, actor
  placement, lip-sync, and motion in one structured operation.
- Model-maker bridge for preparing and registering additional local
  Style-Bert-VITS2 voices.

**Conditional**

- Style-Bert-VITS2, Kokoro, and GPT-SoVITS use external local runtimes or
  sidecars and are not embedded silently into the editor process.
- Available providers can expose install/start guidance and automatic startup;
  missing providers must report an actionable unavailable state.
- Catalog entries for planned provider adapters are not equivalent to completed
  synthesis support.

## Characters and Subculture Workflows

### Character Asset Hub

**Available**

- Folder scanning and classification for Live2D, Spine, MMD, and VRM assets.
- Dependency diagnostics, thumbnail/readiness summaries, feature descriptions,
  recommended transforms/origins, and one-click result templates.
- Action payloads can place compatible assets into timeline or avatar
  workflows.

### Live2D

**Available**

- Model loading, authored motions, expressions/parameters where exposed by the
  asset, natural blink, lip-sync, actor placement, timeline integration, and
  render diagnostics.
- Dialogue and subtitle workflows can drive mouth and motion parameters.
- Public evidence includes a finished 30-second Live2D voice scene.

**Limited**

- Compatibility depends on the authored model and SDK-supported data.
- Tiger Studio does not claim complete compatibility with every extracted or
  modified game asset.

### Spine

**Available**

- Spine asset discovery, skins, animations, placement, timeline actor tracks,
  GPU-oriented preview integration, and compatibility diagnostics.
- Supported samples can be inspected in the dedicated Spine editor.

**Limited**

- Asset version, atlas, attachment, clipping, blend, and custom-runtime
  differences can affect compatibility.
- Original Unity AssetBundle ingestion is not claimed as universal direct
  support.

### MMD

**Available**

- PMX/PMD model and VMD motion workflows, camera fallback/framing, toon
  materials, outlines, shadows, lighting, bloom, material specialization,
  animation, IK/physics paths, and timeline/editor integration.
- Character Hub and MMD Actions expose model/motion setup and diagnostics.

**Limited**

- Compatibility varies with model-specific materials, physics, SDEF, IK,
  transparency, and authored motion assumptions.
- Full reference-runtime parity for every MMD asset is not claimed.

### VRM and VTuber Studio

**Available**

- VRM intake, avatar mapping, source-person framing policy, facial/body motion
  mapping, internal MToon GPU rendering, and Program Output composition.
- VTuber Studio separates Performance Source from final Program Output.
- Broadcast scenes support source/avatar layers, backgrounds, overlays,
  preflight, live-target presets, and evidence capture.
- Internal VRM fallback keeps Program Output available when optional VSeeFace
  integration is absent or degraded.

**Conditional / Limited**

- External streaming targets require platform configuration and credentials.
- VSeeFace remains an optional sidecar, not a normal project dependency.
- Commercial broadcast claims remain gated by real platform evidence and
  sustained runtime performance.

## AR / PBR / 3D

### 3D Asset Preview and Compositing

**Available**

- Media Pool classification and preview for glTF, GLB, VRM, and limited FBX.
- PBR material controls, HDR environment presets, key/ambient lighting,
  metallic/roughness/clearcoat controls, SSAO/contact treatment, shadow and
  reflection catchers, and transform gizmos.
- AR/PBR actor tracks composite over video in preview and export.
- glTF/GLB/VRM geometry is the strongest current support tier.

**Limited**

- FBX conversion and incomplete material sets are reported as limited.
- Unsupported compressed meshes or failed imports return explicit diagnostics
  instead of pretending to render correctly.

### Depth, Placement, and Occlusion

**Available**

- Registered synthetic, local ONNX, external-sequence, and temporal depth
  provider boundaries.
- Depth cache manifests, stale detection, edge refinement, temporal smoothing,
  depth inspection modes, road/floor diagnostics, placement anchors, and
  video-depth occlusion in preview/export paths.
- The viewer Depth control is diagnostic, user-controlled, and off by default.

**Conditional / Limited**

- Production depth quality requires a configured real depth model or external
  depth sequence. Synthetic luminance depth is a deterministic QA fallback.
- The worker-safe full-GPU helper currently applies depth as a post-render
  overlay matte rather than a native helper-side object-depth-buffer compare.

### Texture Map Lab

**Available**

- Image-to-material generation for base color, normal, height, AO, cavity,
  roughness, metallic, and packed map workflows.
- Plane preview, lighting/environment controls, de-light/albedo recovery, and
  Unreal-oriented export conventions.
- Structured `ar_pbr.texture_lab.*` Actions.

### Engine Link

**Limited / Experimental**

- An Unreal-facing structured bridge and Actions exist for handoff and
  automation experiments.
- Full editor-engine project round trip, universal material conversion, and
  production deployment parity are not claimed.

## AI, Actions, and Reviewability

### Studio-Wide Actions

**Available**

Tiger Studio exposes structured, inspectable namespaces for:

- timeline, selection, clip editing, tracks, markers, and media;
- NLE bins, source records, multicam, auditions, storylines, and readiness;
- audio, music, MIDI, TTS, paint, PPT, and Motion Designer;
- Live2D/Spine/MMD/VRM actors, Character Hub templates, VTuber, and broadcast;
- AR/PBR preview, gizmos, depth, Texture Map Lab, and 3D workflows;
- UI, capture evidence, review evidence, project health, and export;
- optional Unreal/engine-link workflows.

Actions return structured state and diagnostics so AI automation can be
reviewed without scraping the UI.

### Local and Connected AI Providers

**Available / Conditional**

- Provider boundaries support local planning and connected agent workflows.
- Clear user intent can route to editable operations such as prompt-to-edit,
  prompt-to-deck, prompt-to-music, dialogue takes, motion generation, and
  Painter operations.
- Consequential edits remain structured and reviewable.
- Provider availability, model installation, credentials, and runtime readiness
  determine which generation backends can run.

### Review Automation and QA

**Available**

- Real editor screenshots, window capture, GIF/video evidence, export bake
  checks, actor compatibility matrices, UI layout checks, project audits,
  performance sampling, and product-readiness reports.
- Public product evidence must come from real Tiger Studio UI or real renderer
  output. Generated design references are not presented as fake product
  screenshots.
- Review automation can build internal reports, sites, and presentation decks;
  it is separate from the user-facing PPT Maker.

## Public Evidence

The public page currently includes:

1. AI full-process editing demo.
2. Finished Live2D commentary output.
3. One-click classical Composer demo.
4. AI Painter brushwork demo.
5. Editorial Motion Graphics demo.
6. Twenty-three product catalog slides covering the editor, media, timeline,
   effects, typography, color, nodes, audio, actors, AR/PBR, creator assistance,
   and export.

## Product Claim Boundaries

Tiger Studio does not currently claim:

- Premiere Pro, DaVinci Resolve/Fusion/Fairlight, After Effects, Photoshop,
  Cubism, Spine Runtime, PowerPoint, a professional DAW, OBS, or VTube Studio
  feature parity;
- cloud-first multi-user collaboration comparable to mature web platforms;
- compatibility beyond the measured actor and 3D asset corpus; extracted
  Unity, Live2D, Spine, MMD, VRM, FBX, and game assets remain
  format- and authoring-dependent;
- production-quality monocular video depth without a configured real model;
- every optional TTS, music, AI, broadcast, office, or engine sidecar being
  installed and ready by default;
- universal real-time performance for every dense character or 3D asset.

The product position is integration: creator-facing editing, character,
presentation, voice, music, motion, paint, broadcast, and 3D workflows share
one local project and one structured automation surface.

## Public Catalog Image Order

1. `01_studio_overview.png`
2. `02_studio_surface.png`
3. `03_ai_workflow.png`
4. `04_ppt_maker.png`
5. `05_media_pool.png`
6. `06_timeline.png`
7. `07_effects.png`
8. `08_transitions.png`
9. `09_typography.png`
10. `10_keyframes.png`
11. `11_color.png`
12. `12_node_graph.png`
13. `13_node_effects.png`
14. `14_music_lab.png`
15. `15_audio_workbench.png`
16. `16_audio_curves.png`
17. `17_live2d_spine.png`
18. `18_vrm.png`
19. `19_mmd.png`
20. `20_ar_pbr.png`
21. `21_creator_assist.png`
22. `22_export.png`
23. `23_closing.png`

## Distribution Boundary

The public repository contains distribution-safe pages, documentation, catalog
images, demo media, release notes, installers, and packaged artifacts only.
Source code is maintained separately.

Public Windows downloads remain paused until the packaged build passes the
current release-readiness, packaging, and distribution gates.
