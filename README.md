# Skills

Small, reusable instructions that help an AI agent approach a task. Each skill lives in its own folder, with a `SKILL.md` that says when to use it and what to do.

## Skills

- [Be more pedagogical](skills/be-more-pedagigical/) — explain ideas clearly, at the reader's level.
- [Document a skill](skills/document-skill/) — add or update a skill in this repository.

## Use a skill

In Codex, ask the skill installer to install a skill from its GitHub folder. For example:

```text
Use $skill-installer to install https://github.com/MrEmanuel/skills/tree/master/skills/be-more-pedagigical
```

The skill is available on your next turn. You can invoke it by name, for example `$be-more-pedagigical`, or let Codex use it when relevant. Other agents that support the [Agent Skills format](https://agentskills.io/) can use the same folders; follow your agent's installation instructions.

## Add a skill

Create `skills/<skill-name>/SKILL.md` with a name, description, and instructions. Add supporting files only when needed, and link the skill in the list above. The [document a skill](skills/document-skill/SKILL.md) skill guides this process.

## License

[MIT](LICENSE)
