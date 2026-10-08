# skills

**English** · [中文](README.zh.md)

A collection of reusable skills for AI agents.

Each folder under [`skills/`](skills/) is one self-contained skill: a `SKILL.md` that tells the
assistant when and how to use it, plus the files it needs. Everything is plain Markdown, so the
skills work with any assistant that can read files.

## Skills

| Skill | What it does | Languages |
|---|---|---|
| [Founder Guide · 创业参谋](skills/founder-guide/) | Twelve situation-based playbooks for the decisions founders get stuck on: demand validation, MVP scope, pricing, early growth, B2B sales, competing with incumbents, equity and co-founders, hiring and firing, managing a team, negotiation, judging claims and forecasts, and crisis decisions. | English, 中文 |

## How to use a skill

1. **Download.** Click the green **Code** button on this page → **Download ZIP**, and unzip it.
2. **Agents with skill support.** Copy the skill's folder (for example `skills/founder-guide/`)
   into the directory your agent loads skills from, keeping the folder name.
3. **Chat apps without skill support.** Paste the contents of the skill's `SKILL.md` into the
   app's custom instructions (or project instructions), and upload the rest of that folder as
   project files.

Each skill's own README has the details.

## License

[MIT](LICENSE)
