# claude-simple-qa

A [Claude Code](https://code.claude.com) plugin marketplace with one plugin: **simple-qa**.

## simple-qa

Type `/simple-qa` once, and every later answer in the session comes back in
simple English, as at most three short bullet points.

The rules Claude follows after you invoke it:

- Use simple English.
- Define each new term first, then use that same term every time; never swap in a synonym.
- Answer in bullet points, so the answer is easy to scan.
- Write at most three bullets, each with few words, and make them read as one coherent answer.

### Install

From inside Claude Code:

```
/plugin marketplace add darshankapashi/claude-simple-qa
/plugin install simple-qa@claude-simple-qa
```

Then enable it from `/plugin`. No `settings.json` editing required.

### Use

```
/simple-qa
```

It takes no arguments and lasts for the rest of the session. Start a new
session to get normal answers back.

> If you already have a `simple-qa` skill in `~/.claude/skills/` or a project's
> `.claude/skills/`, remove one of them so the two don't shadow each other.

## License

MIT
