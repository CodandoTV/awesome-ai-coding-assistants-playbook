# AI Contribution Rules

This file defines the shared rules for AI coding assistants maintaining and updating this repository.
Follow these guidelines in every session without needing to be reminded.

---

## Repository Purpose

A centralized map of references for configuring AI coding assistants.
Covers: skills, instructions, prompts, agents, rules, SDD tools and AI coding assistants.

**This is a map — not a catalog.**
We point to repos and resources, we do not host skills or prompts directly.
Only add resources that are specifically about configuring AI coding assistants.
Do NOT add: AI frameworks, ML libraries, models, papers or general AI tools.

---

## Tags

Only add a tag when official support is **confirmed**. Do not guess.

**Always use image badges from `BADGES.md` — never plain text tags.**

### Assistant Tags
| Tag | Assistant |
|-----|-----------|
| `claude` | [Claude Code](https://claude.ai/code) — Anthropic |
| `copilot` | [GitHub Copilot](https://github.com/features/copilot) — GitHub |
| `cursor` | [Cursor](https://www.cursor.com/) |
| `gemini` | [Gemini CLI](https://github.com/google-gemini/gemini-cli) — Google |
| `codex` | [Codex CLI](https://github.com/openai/codex) — OpenAI |
| `windsurf` | [Windsurf](https://windsurf.com/) — Codeium |
| `opencode` | [OpenCode](https://opencode.ai/) |

### Pricing Tags
| Tag | Meaning |
|-----|---------|
| `free` | Has a free tier |
| `paid` | Paid only |
| `open source` | Source code is publicly available and freely modifiable |

---

## Sections

| Section | What belongs here |
|---------|------------------|
| Skills | SKILL.md repos and skill collections |
| Instructions & Rules | `.cursorrules`, `copilot-instructions.md`, rule files |
| Agents | Agent `.md` files, agent collections |
| System Prompts | Reverse-engineered or reference system prompts |
| Prompts & Templates | Prompt engineering resources and templates |
| Tools | SDD tools and skill/config management tools |
| AI Coding Assistants | The assistants themselves — not configs |
| Content | Videos, posts and talks about the topic |

---

## Adding a Resource

Each entry must follow this format:

```markdown
- **[owner/repo](https://github.com/owner/repo)** `tag1` `tag2`  
  > One-line description of what it is and why it's relevant
```

Rules:
- Description must be in English
- Keep descriptions short — one line only
- Only add tags you are certain about
- Place in the correct section
- For paid tools, always add `free` or `paid` tag

---

## Content Section

The Content section has two subsections:

- **CodandoTV** — videos from the CodandoTV YouTube channel
- **Community** — videos, posts or talks from anyone in the community

Format for videos:
```markdown
- **[Video Title](https://youtube.com/...)**
```

---

## Bilingual Files

This repo has English and Portuguese (PT-BR) versions of key files:

| English | Portuguese |
|---------|-----------|
| `README.md` | `README.pt-br.md` |
| `CONTRIBUTING.md` | `CONTRIBUTING.pt-br.md` |
| `AI_INSTRUCTIONS.md` | `AI_INSTRUCTIONS.pt-br.md` |

**Rule: whenever you update the English version, you MUST update the PT-BR version in the same session.**
Never leave the two versions out of sync.

---

## What NOT to add

- AI frameworks (LangChain, LlamaIndex, etc.)
- ML models or model repos
- On-device AI / edge AI libraries
- General awesome-lists not related to coding assistant configuration
- Tools without clear relation to AI coding assistant configuration
