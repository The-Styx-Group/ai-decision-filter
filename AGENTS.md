# AI Decision Filter — Agent Operating Instructions

Operating context and governance for AI agents working in the `ai-decision-filter` repository.

## 1. Overview & Architecture
- **Purpose:** A multi-agent plugin package (for ChatGPT and Codex) by The Styx Group LLC that evaluates whether a small business process should adopt AI or if conventional process improvement is the proper solution.
- **Repository Structure:**
  - `.agents/plugins/marketplace.json` — Marketplace registration metadata.
  - `plugins/ai-decision-filter/.codex-plugin/plugin.json` — Codex plugin configuration and manifest.
  - `plugins/ai-decision-filter/skills/ai-decision-filter/` — Primary skill definition (`SKILL.md`) and supporting decision references (`references/decide.md`, `tiers.md`, `intake.md`, `diagrams.md`).
  - `plugins/ai-decision-filter/skills/process-re-review/` — Secondary skill for auditing and updating prior process decisions.

## 2. Plugin & Skill Invariants
- **Multi-Platform Consistency:** Changes to skill interfaces or descriptions must be synchronized between the `.agents/` marketplace manifests and the `.codex-plugin/` manifest.
- **Decision Philosophy:** The filter must maintain a skeptical, pragmatic stance. AI is NOT recommended if simple workflow simplification, checklist discipline, or existing software tools solve the issue.
- **Reference Integrity:** The decision trees in `references/decide.md` and `references/tiers.md` govern output scoring. Keep guidance grounded in these schemas.

## 3. Definition of Done
Before completing any task:
1. JSON syntax in `marketplace.json` and `plugin.json` validates cleanly.
2. Changes to `SKILL.md` adhere to agent skill standards (clean frontmatter, clear trigger rules).
3. Any added reference docs are properly linked and referenced in the skill prompts.
