# TigerCapture Public Product Spec

This document is a public, release-safe summary of the current TigerCapture
product direction. It avoids private implementation notes and focuses on the
features shown in the product catalog screenshots.

## Product Position

TigerCapture is a local-first creator studio that combines screen capture,
timeline editing, presentation creation, 3D/AR compositing, character actors,
audio work, and AI-operable review automation.

The product is designed for creators who need to capture work, explain it,
edit it, add visual evidence, and publish a polished video or presentation
without moving through several disconnected tools.

## Core Areas

### Studio Surface

- Main editor with media pool, preview, timeline, inspector/workbench panels,
  transport controls, and status surfaces.
- Dense production UI intended for repeated editing work rather than a
  marketing-first landing screen.
- Review automation can capture real UI states for product evidence.

### Timeline Editing

- Multi-track timeline for video, audio, typography, effects, transitions,
  actor/3D assets, and presentation-style material.
- Clip status badges and thumbnail treatments communicate effects, transitions,
  color grading, and track state.
- Drag-and-drop workflows are preferred for media pool to timeline operations.

### PPT Maker

- Independent presentation editor prototype designed to integrate with the
  existing TigerCapture media pool and timeline ecosystem.
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

### AI-Operable Actions

- TigerCapture exposes structured Python Action / MCP-style surfaces so local
  AI or review automation can inspect project state and operate features.
- Review automation must use real TigerCapture UI screenshots and real rendered
  proof outputs for product evidence.

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
14. `14_audio_workbench.png`
15. `15_audio_curves.png`
16. `16_live2d_spine.png`
17. `17_vrm.png`
18. `18_mmd.png`
19. `19_ar_pbr.png`
20. `20_creator_assist.png`
21. `21_export.png`
22. `22_closing.png`

## Release Notes Boundary

This public distribution repository should contain release-safe pages,
screenshots, installers, and metadata. Installer binaries are distributed
through GitHub Releases.
