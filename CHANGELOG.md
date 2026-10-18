# CHANGELOG.md — Important Development History

## [1.1.14] - 2026-10-18
- **Milestone**: Implementation of AI-Independent Development Continuity System and multi-vertical business switcher (Restaurant, Kirana, Medical, Garment, Electronics, etc.).
- **Summary of Changes**:
  - Added project memory files (`AGENTS.md`, `PROJECT_CONTEXT.md`, `CURRENT_TASK.md`, `CHANGELOG.md`, `TESTING.md`).
  - Added REST API endpoint `/api/business/switch-vertical` and restaurant table initialization.
  - Enhanced Settings view with interactive business vertical selector and capability highlights.
  - Resolved all TypeScript and ESBuild compilation issues.
- **Verification**: `npm run build` and `tsc --noEmit` passed successfully with zero errors.
