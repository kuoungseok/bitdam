# Tiger Studio Public Product Spec

This document is a public, release-safe summary of the current Tiger Studio
product direction. Tiger Studio was formerly called TigerCapture; the public
repository still uses the `tigercapture` name for distribution continuity.
This page focuses on release-safe product behavior shown in the product catalog
screenshots.

## Product Position

Tiger Studio is a subculture-ready video editor for screen, shorts, and
character creators. It combines screen-recording polish, timeline editing,
presentation pages, 3D/AR compositing, Live2D/Spine/MMD/VRM character actors,
audio work, and reviewable AI-assisted workflows.

The product is designed for creators who need to capture or import footage,
edit it, add characters or voice/music/presentation material, and publish a
polished video without moving through several disconnected tools.

Korean: 화면녹화, 쇼츠, 캐릭터 영상, 음성, 음악, 발표 페이지를 하나의 로컬 우선
영상편집 흐름으로 묶는 것이 핵심입니다.

## Core Areas

### Timeline Video Editor

- Main editor with media pool, preview, timeline, inspector/workbench panels,
  transport controls, and status surfaces.
- Dense production UI intended for repeated editing work rather than a simple
  capture utility.
- Public screenshots use real editor states for product evidence.

### Timeline Editing

- Multi-track timeline for video, audio, typography, effects, transitions,
  actor/3D assets, and presentation-style material.
- Clip status badges and thumbnail treatments communicate effects, transitions,
  color grading, and track state.
- Drag-and-drop workflows are preferred for media pool to timeline operations.

### PPT / Presentation Pages

- Independent presentation editor prototype designed to integrate with the
  existing Tiger Studio media pool and timeline ecosystem.
- Video, 3D, and typography assets can become slide actors through
  drag-and-drop workflows.
- Timeline-style thinking can be used to create frame/page-based presentation
  sequences.

### Color, Effects, and Nodes

- Color grading, effect badges, node-style effect flows, and before/after
  review surfaces are treated as first-class editor features.
- Public screenshots show color, node graph, node effects, transitions, and
  timeline evidence.

### Audio and Music Lab

- Sound Editor workbench includes audio controls, dynamics-style workflow, and
  AI-assisted music generation planning.
- Music Lab is MIDI-first for editable composition structure, then renders WAV
  previews/stems through configured local or external renderers.
- Built-in renderers are draft/starter previews. Modern production-quality
  music requires a configured production renderer or licensed sample/model
  backend.

### AR / PBR / 3D

- 3D assets can be imported and previewed through the AR/PBR workflow.
- Depth-aware video compositing is part of the product direction, including
  occlusion and preview/export parity targets.
- The renderer path is intended to support higher quality PBR previews rather
  than flat placeholder meshes.

### Actors: Live2D, Spine, VRM, MMD

- Character workflows are represented as editable actors, not just external
  overlays.
- MMD and VTuber/VRM paths are tracked as product areas with their own rendering
  and material concerns.
- Public catalog slides include Live2D/Spine, VRM, and MMD evidence pages.

### AI Actions and Automation

- Tiger Studio exposes structured action surfaces so local AI and review
  automation can inspect project state and operate editor features safely.
- Review/catalog evidence must use real Tiger Studio UI screenshots and real
  rendered proof outputs.

## Public Catalog Image Order

1. `02_studio_surface.png`
2. `03_ai_workflow.png`
3. `04_ppt_maker.png`
4. `05_media_pool.png`
5. `06_timeline.png`
6. `07_effects.png`
7. `08_transitions.png`
8. `09_typography.png`
9. `10_keyframes.png`
10. `11_color.png`
11. `12_node_graph.png`
12. `13_node_effects.png`
13. `14_audio_workbench.png`
14. `15_audio_curves.png`
15. `16_live2d_spine.png`
16. `17_vrm.png`
17. `18_mmd.png`
18. `19_ar_pbr.png`
19. `20_creator_assist.png`
20. `21_export.png`
21. `22_closing.png`

## Release Notes Boundary

This public distribution repository should contain release-safe pages,
screenshots, installers, and metadata. Public installer downloads are
temporarily paused until the current packaged build passes release-readiness
gates.
