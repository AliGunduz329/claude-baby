# Claude Baby ✍️

A curated engine of rules, anti-patterns, and few-shot exemplars designed to de-slop LLM writing.

## Repository Layout

- **`CLAUDE.md`**: Master system-level prompt and anti-patterns automatically consumed by Claude.
- **`style_guide/`**: In-depth rules on diction, rhythm, sentence variation, and the **banned phrases** blacklist.
- **`system_prompts/`**: Modular prompt templates (e.g., `editing_pass.md`) for revising rough drafts.
- **`exemplars/`**: Side-by-side bad vs. good rewrites showing the exact mechanics of strong prose.
- **`evals/`**: Benchmark prompts used to test Claude against formulaic phrasing, AI tells, and hollow transitions.

## How to Deploy in Claude Projects
1. Copy the contents of `CLAUDE.md` and `style_guide/banned_phrases.md` into **Project Instructions**.
2. Add files from `exemplars/` and `style_guide/` into **Project Knowledge**.
3. Use `system_prompts/editing_pass.md` whenever you need an exacting critique of a rough draft.
