# AI Decision Filter — Agent Operating Instructions

Operating context and governance for AI agents working in the `ai-decision-filter` repository.

## 1. Overview & Architecture
- **Purpose:** A ChatGPT/Codex plugin with two skills, by The Styx Group LLC, that evaluates whether a small business process should adopt AI or if conventional process improvement is the proper solution.
- **Repository Structure:** see `README.md` → What's inside. Marketplace registration lives in `.agents/plugins/marketplace.json`.

## 2. Plugin & Skill Invariants
- **Multi-Platform Consistency:** The plugin `name`, `interface.displayName` and category (`plugins[].category` in the marketplace file, `interface.category` in plugin.json) must match between `.agents/plugins/marketplace.json` and `plugins/ai-decision-filter/.codex-plugin/plugin.json`.
- **Decision Philosophy:** The filter must maintain a skeptical, pragmatic stance. AI is NOT recommended if simple workflow simplification, checklist discipline, or existing software tools solve the issue.
- **Reference Integrity:** The decision trees in `references/decide.md` and `references/tiers.md` govern output scoring. Keep guidance grounded in these schemas.

## 3. Definition of Done
Before completing any task:
1. JSON syntax in `marketplace.json` and `plugin.json` validates cleanly.
2. Changes to `SKILL.md` adhere to agent skill standards (clean frontmatter, clear trigger rules).
3. Any added reference docs are properly linked and referenced in the skill prompts.
