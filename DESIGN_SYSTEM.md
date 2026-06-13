# CFI Coach -- Design System Spec

Status: spec only, not yet implemented. Current build (index.html, teach-back.html, styles.css) uses a single theme and an 11-phase flow (Overview through Pass/Retry). This document is the target design system for future work.

## Dual-Theme Cognitive Design

**Light mode -- Learning Phases**
- Off-White #F7F7F7
- White #FFFFFF
- Light Gray #E4E4E4
- Dark Navy accents #1A2A3A

**Dark mode -- Performance Phases**
- Deep Navy #1A2A3A
- Charcoal #1F1F1F

**Shared accents (both themes)**
- Sky Blue #4DA3FF
- Mint #6EE7B7

Rules:
- Light mode = clarity, energy, readability (used for learning/intake phases).
- Dark mode = immersion, calm, cockpit-authentic (used for performance/evaluation phases).
- Accent colors are constant across both themes to unify the brand.

## 12-Phase Lesson Flow

1. Overview (light)
2. Video (light)
3. Written Lesson -- 3-5 bullets + simple diagram (light)
4. Flashcards (light)
5. Quiz -- 3-5 questions + explanations (light)
6. Teach-Back -- whiteboard + audio recording (dark)
7. Feedback -- AI critique + FAA citations (dark)
8. Mini-Lesson -- 2-4 sentence correction (dark)
9. Student Question -- scenario misunderstanding (dark)
10. Reteach -- user teaches again (dark)
11. Pass/Retry -- ACS-aligned evaluation (dark)
12. Summary -- 3-5 takeaways + FOI tie-in (light)

Note: phases 6-11 are implemented in teach-back.html today as TEACH_BACK, FEEDBACK, MINI_LESSON, FOLLOW_UP_QUESTION, RETEACH, PASS_RETRY_DECISION. Phase 12 (Summary) is not yet built.

## Layout Principles

- **Vertical Lesson Flow** (medical-style): clean, scroll-based, low cognitive load.
- **Strong Topbar** (legal-style): phase badge, lesson title, progress indicator.
- **Whiteboard as Primary Element** (pilot-style): large, high contrast, minimal chrome.
- **FAA Source Drawer** (unique): collapsible, includes AIH, PHAK, AFH, ACS references; inline citations required in feedback phases.
- **Component style**: rounded cards, soft shadows, modern premium minimalism, consistent spacing rhythm.

## Output Requirements for Design Work

When implementing or revising screens against this system, cover:
1. Screen layout (structure, hierarchy, spacing)
2. Color usage (light or dark theme + accents)
3. Component descriptions (cards, buttons, headers, whiteboard)
4. Typography system (weights, sizes, roles)
5. Interaction patterns (how the user moves through the phase)
6. Cognitive justification (why this design improves learning/performance)
7. How accent colors unify the brand across themes

Decisions should reference: cognitive load, aviation authenticity, FOI principles, ACS performance standards, and dual-theme consistency.
