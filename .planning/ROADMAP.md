# Roadmap: ZSM Usability Improvements

## Overview

Polish ZSM's visual presentation and interaction patterns across six focused phases — from color refinement through responsive feedback — making the session selector feel instant and intuitive.

## Domain Expertise

None

## Phases

**Phase Numbering:**
- Integer phases (1, 2, 3): Planned milestone work
- Decimal phases (2.1, 2.2): Urgent insertions (marked with INSERTED)

- [x] **Phase 1: Color Palette** - Replace harsh pink/magenta with muted colors for live sessions
- [x] **Phase 2: MRU Ordering** - Sessions ordered by most recent switch with config option
- [x] **Phase 3: Tabular Alignment** - Session names and directories in clean columns
- [ ] **Phase 4: Title Update** - Change title to "ZSM - Zellij Session Manager"
- [ ] **Phase 5: Responsive Deletion** - Immediate UI feedback when killing sessions
- [ ] **Phase 6: Help Text Layout** - Two-row help text with logical grouping

## Phase Details

### Phase 1: Color Palette
**Goal**: Replace harsh pink/magenta bullet indicators with subtle, muted colors that complement the cyan session names
**Depends on**: Nothing (first phase)
**Research**: Unlikely (internal UI theming in src/ui/theme.rs and src/ui/components.rs)
**Plans**: TBD

Plans:
- [x] 01-01: Update theme colors for live session indicators

### Phase 2: MRU Ordering
**Goal**: Sort sessions by most recent switch rather than alphabetically, with a config option to choose sort order
**Depends on**: Phase 1
**Research**: Unlikely (state management in src/state.rs, config in src/config.rs)
**Plans**: TBD

Plans:
- [x] 02-01: Add sort_order config option
- [x] 02-02: Implement MRU tracking and ordering

### Phase 3: Tabular Alignment
**Goal**: Align session names and directory paths in clean columns for improved readability
**Depends on**: Phase 2
**Research**: Unlikely (renderer changes in src/ui/renderer.rs)
**Plans**: TBD

Plans:
- [x] 03-01: Implement columnar layout for session list

### Phase 4: Title Update
**Goal**: Change plugin title from current to "ZSM - Zellij Session Manager"
**Depends on**: Phase 3
**Research**: Unlikely (simple string change in renderer)
**Plans**: TBD

Plans:
- [ ] 04-01: Update title string in renderer

### Phase 5: Responsive Deletion
**Goal**: Provide immediate visual feedback when deleting sessions to reduce perceived lag
**Depends on**: Phase 4
**Research**: Unlikely (session manager patterns in src/session/manager.rs)
**Plans**: TBD

Plans:
- [ ] 05-01: Add optimistic UI update on delete action

### Phase 6: Help Text Layout
**Goal**: Reorganize help text into two rows with navigation keys on row 1, action keys on row 2
**Depends on**: Phase 5
**Research**: Unlikely (renderer component layout)
**Plans**: TBD

Plans:
- [ ] 06-01: Restructure help text rendering

## Progress

**Execution Order:**
Phases execute in numeric order: 1 → 2 → 3 → 4 → 5 → 6

| Phase | Plans Complete | Status | Completed |
|-------|----------------|--------|-----------|
| 1. Color Palette | 1/1 | Complete | 2026-01-14 |
| 2. MRU Ordering | 2/2 | Complete | 2026-01-13 |
| 3. Tabular Alignment | 1/1 | Complete | 2026-01-13 |
| 4. Title Update | 0/1 | Not started | - |
| 5. Responsive Deletion | 0/1 | Not started | - |
| 6. Help Text Layout | 0/1 | Not started | - |
