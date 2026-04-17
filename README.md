# humanmade

A Claude Code skill for writing prose that reads as authentically human. With a special focus on scientific research and large bodies of text.

Combines three capabilities into one skill:

1. **Human voice** — banned AI vocabulary, sentence pattern rules, significance inflation kills, tone and structural guidelines distilled from Wikipedia's field guide to AI-generated content
2. **Scientific writing** — IMRAD structure, citation styles (APA/AMA/Vancouver/Chicago/IEEE), figures/tables, reporting guidelines (CONSORT/STROBE/PRISMA), LaTeX report formatting
3. **Critical thinking** — methodology critique, bias detection, statistical evaluation, evidence quality (GRADE), claim evaluation, logical fallacy identification

## Install

```bash
git clone https://github.com/machinemade-mm/humanmade-antislop.git && cp -r humanmade-antislop ~/.claude/skills/humanmade
```

## Usage

In Claude Code:

```
/humanmade
```

Then write normally. The skill applies human-voice rules to all output and activates scientific writing and critical thinking layers when relevant.

## Credits

This is an original work that distills and consolidates insights from multiple sources into a new, unified skill. Inspirations and source material include:

- [Wikipedia: Signs of AI-generated content](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI-generated_content)
- Scientific writing and critical thinking skills by [K-Dense Inc.](https://github.com/k-dense)

## License

MIT
