# Regras de Contribuição de IA

Este arquivo define as regras compartilhadas para assistentes de codificação de IA que mantêm e atualizam este repositório.
Siga estas diretrizes em cada sessão sem precisar ser lembrado.

---

## Propósito do Repositório

Um mapa centralizado de referências para configurar assistentes de codificação de IA.
Cobre: skills, instruções, regras, prompts, agentes, ferramentas SDD e assistentes de codificação de IA.

**Este é um mapa — não um catálogo.**
Apontamos para repositórios e recursos, não hospedamos skills ou prompts diretamente.
Adicione apenas recursos que sejam especificamente sobre a configuração de assistentes de codificação de IA.
NÃO adicione: frameworks de IA, bibliotecas de ML, modelos, artigos ou ferramentas gerais de IA.

---

## Tags

Adicione uma tag apenas quando o suporte oficial for **confirmado**. Não adivinhe.

**Sempre use badges de imagem do `BADGES.md` — nunca tags de texto simples.**

### Tags de Assistente
| Tag | Assistente |
|-----|-----------|
| `claude` | [Claude Code](https://claude.ai/code) — Anthropic |
| `copilot` | [GitHub Copilot](https://github.com/features/copilot) — GitHub |
| `cursor` | [Cursor](https://www.cursor.com/) |
| `gemini` | [Gemini CLI](https://github.com/google-gemini/gemini-cli) — Google |
| `codex` | [Codex CLI](https://github.com/openai/codex) — OpenAI |
| `windsurf` | [Windsurf](https://windsurf.com/) — Codeium |
| `opencode` | [OpenCode](https://opencode.ai/) |

### Tags de Preço
| Tag | Significado |
|-----|---------|
| `free` | Possui nível gratuito |
| `paid` | Apenas pago |
| `open source` | Código fonte disponível publicamente e livremente modificável |

---

## Seções

| Seção | O que pertence aqui |
|---------|------------------|
| Skills | Repositórios SKILL.md e coleções de skills |
| Instructions & Rules | Arquivos `.cursorrules`, `copilot-instructions.md`, arquivos de regras |
| Agents | Arquivos `.md` de agentes, coleções de agentes |
| System Prompts | System prompts de referência ou engenharia reversa |
| Prompts & Templates | Recursos de engenharia de prompt e templates |
| Tools | Ferramentas SDD e ferramentas de gerenciamento de skill/config |
| AI Coding Assistants | Os assistentes em si — não configurações |
| Content | Vídeos, posts e palestras sobre o tópico |

---

## Adicionando um Recurso

Cada entrada deve seguir este formato:

```markdown
- **[owner/repo](https://github.com/owner/repo)** `tag1` `tag2`  
  > Descrição de uma linha sobre o que é e por que é relevante
```

Regras:
- A descrição deve ser em inglês
- Mantenha as descrições curtas — apenas uma linha
- Adicione apenas tags das quais você tem certeza
- Coloque na seção correta
- Para ferramentas pagas, sempre adicione a tag `free` ou `paid`

---

## Seção de Conteúdo

A seção de Conteúdo tem duas subseções:

- **CodandoTV** — vídeos do canal CodandoTV no YouTube
- **Community** — vídeos, posts ou palestras de qualquer pessoa da comunidade

Formato para vídeos:
```markdown
- **[Título do Vídeo](https://youtube.com/...)**
```

---

## Arquivos Bilíngues

Este repositório possui versões em inglês e português (PT-BR) dos arquivos principais:

| Inglês | Português |
|---------|-----------|
| `README.md` | `README.pt-br.md` |
| `CONTRIBUTING.md` | `CONTRIBUTING.pt-br.md` |
| `AI_INSTRUCTIONS.md` | `AI_INSTRUCTIONS.pt-br.md` |

**Regra: sempre que você atualizar a versão em inglês, você DEVE atualizar a versão PT-BR na mesma sessão.**
Nunca deixe as duas versões fora de sincronia.

---

## O que NÃO adicionar

- Frameworks de IA (LangChain, LlamaIndex, etc.)
- Modelos de ML ou repositórios de modelos
- Bibliotecas de IA on-device / edge IA
- Listas "awesome" gerais não relacionadas à configuração de assistentes de codificação
- Ferramentas sem relação clara com a configuração de assistentes de codificação de IA
