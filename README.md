# Skills

Small, reusable instructions that help an AI agent approach a task. Each skill lives in its own folder, with a `SKILL.md` that says when to use it and what to do.

## Skills

- [Be more pedagogical](skills/be-more-pedagigical/) — explain ideas clearly, at the reader's level.
- [Document a skill](skills/document-skill/) — add or update a skill in this repository.

## Install

Clone this repository, then copy the **whole skill folder** into your project's skills directory:

```sh
git clone https://github.com/MrEmanuel/skills.git
```

| Agent | Project skills directory |
| --- | --- |
| [Codex](https://learn.chatgpt.com/docs/build-skills) | `.agents/skills/` |
| [GitHub Copilot](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/add-skills) | `.github/skills/` |
| [Claude Code](https://code.claude.com/docs/en/skills) | `.claude/skills/` |
| [Cursor](https://cursor.com/docs/skills) | `.cursor/skills/` |
| [Gemini CLI](https://geminicli.com/docs/cli/skills/) | `.gemini/skills/` |
| [OpenCode](https://opencode.ai/docs/skills/) | `.opencode/skills/` |

For example, copy `skills/skills/be-more-pedagigical/` from the clone to your project's chosen directory, so it contains `be-more-pedagigical/SKILL.md`. Start a new agent session to use it.

For Codex, you can also ask: `Use $skill-installer to install https://github.com/MrEmanuel/skills/tree/master/skills/be-more-pedagigical`.

## Add a skill

Create `skills/<skill-name>/SKILL.md` with a name, description, and instructions. Add supporting files only when needed, and link the skill in the list above. The [document a skill](skills/document-skill/SKILL.md) skill guides this process.

## License

[MIT](LICENSE)
