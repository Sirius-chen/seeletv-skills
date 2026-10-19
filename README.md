# seeletv-skills

Focused English-language skills for short-form story development, visual reference assets, and directed video prompts.

| Skill | Use it for |
|---|---|
| [seeletv-story](skills/seeletv-story/SKILL.md) | Develop an idea, write a short screenplay, diagnose a scene, or make a constrained rewrite. |
| [seeletv-assets](skills/seeletv-assets/SKILL.md) | Establish visual direction and prepare consistent character, location, and prop references. |
| [seeletv-shots](skills/seeletv-shots/SKILL.md) | Write timed video prompts with camera placement, movement, blocking, performance, sound, and continuity. |

Each entrypoint stays short. Detailed craft guidance is loaded from the relevant local references. The skills work independently from material supplied in the conversation or through available host tools; no canvas graph, fixed project layout, state-recovery skill, or new generation backend is required.

## Installation

Copy the desired directories under `skills/` into your agent's skills directory. For Codex, the default is `~/.codex/skills/`. `seeletv-assets` replaces the earlier `seeletv-assets-trial` package.

## Usage

```text
Use $seeletv-story to turn this idea into a 40-second scene, keeping the ending I specified.

Use $seeletv-assets to establish the visual direction and prepare only the reference assets this scene needs.

Use $seeletv-shots to write a 12-second video prompt with explicit cuts, camera placement, acting, and continuity.
```

Prompt preparation does not submit paid generation tasks. Actual generation uses the host's available tools when authorized. Model-specific syntax and limits must be verified against the actual interface rather than inferred from the model name.

## Sources

The guidance was selectively rewritten and reorganized from the sources identified in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md). Upstream marketing, installers, broad workflow systems, quoted craft-book passages, and fixed aesthetic formulas are not bundled into the skills. Source notices and applicable license texts are kept separately from agent instructions.
