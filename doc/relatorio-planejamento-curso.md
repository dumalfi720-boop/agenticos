# Relatório de Planejamento — Curso Agentic OS

Data: 2026-05-10
Autor: Nei Maldaner + Claude (Opus 4.7)

---

## 1. Leitura crítica da tese

**Tese original do Nei:** "Agentic OS é o sistema operacional do futuro; n8n e outras soluções são apenas as linguagens para construir esses sistemas."

**Veredito:** Direção correta, mas precisa de refinamento técnico.

### Quadro preciso — hierarquia de camadas

| Era clássica | Era agêntica |
|---|---|
| Hardware (CPU, RAM, disco) | LLMs (Claude, GPT, Gemini) + tokens + contexto |
| Kernel / SO (Linux, Windows) | **Agentic OS** (CLAUDE.md, skills, hooks, orquestrador, memória, identidade) |
| Protocolos (TCP/IP, POSIX) | **MCP**, A2A, OpenAPI, agent protocols |
| Linguagens (C, Python, JS) | **n8n, Make, LangGraph, Python+SDK, Claude Code, Cursor** |
| Aplicações (Word, Photoshop) | Agentes especializados (CFO Bot, Researcher, Builder...) |
| Sistemas de arquivos | Silver Platters + RAG + vector stores + memória |
| Cron, daemons | Hooks, schedules, watchers, event triggers |

### Frase de posicionamento técnico

> **n8n, Make, LangGraph, Claude Code são linguagens/IDEs. Agentic OS é o sistema operacional. MCP é o protocolo. LLM é o hardware semântico.**

### Camada que faltava na tese inicial

**MCP (Model Context Protocol)** — está virando o "TCP/IP da era agêntica". Sem cobrir isso, o curso não fica à frente.

---

## 2. Visão de futuro — onde o curso precisa ir mais longe

Sete ângulos que ninguém no mercado BR está vendendo ainda:

1. **Personal Agentic OS vs Enterprise Agentic OS** — assim como Windows vs Unix, vão existir SOs agênticos para indivíduos (Claude Code + skills locais) e para empresas (orquestração multi-agente com governança).
2. **Memory é o novo filesystem** — Silver Platters hoje são `.md`. Amanhã são memória contextual versionada, com TTL, escopo e ACLs.
3. **Hooks = interrupts** — assim como SOs clássicos têm interrupts de hardware, Agentic OS tem hooks (SessionStart, PostToolUse, Stop) que dão previsibilidade ao não-determinístico.
4. **Identidade > prompt** — CLAUDE.md / AGENTS.md / system cards são o "passwd" da era agêntica. Quem é o agente, o que pode tocar, qual sua jurisdição.
5. **Governança e auditoria viram first-class citizens** — não é mais "logging opcional", é parte do kernel.
6. **Orquestração hierárquica vence orquestração plana** — o mercado caminha pra "chief-of-staff pattern" (Anthropic já documenta).
7. **Compute substitutivo, não aditivo** — Agentic OS não automatiza tarefas, ele **substitui processos inteiros** (ex.: o briefing semanal do Marco não é "automatizado", o cargo de quem fazia briefing é redefinido).

**Esse é o ângulo "melhor mente do mercado"** — porque ninguém no Brasil tá vendendo curso com esse enquadramento. O mercado BR vende "Claude Code do zero" ou "imersão de 1 dia". Ninguém vende **arquitetura de SO**.

---

## 3. Estrutura proposta do curso

### Nome sugerido

**Agentic OS — O Sistema Operacional do Trabalho com IA**
*Subtítulo: Do caos das ferramentas à arquitetura de agentes*

(Alternativa para SEO: "Claude Code Agentic OS")

### Trilhas (6 trilhas mapeadas para as cores INEMA.CLUB)

- **T1 — Fundamentos do Agentic OS** (emerald) — a tese, a filosofia, o futuro
- **T2 — Camada de Identidade** (blue) — CLAUDE.md, AGENTS.md, regras, escopo
- **T3 — Camada de Conhecimento** (purple) — Silver Platters, skills, MCP, RAG
- **T4 — Camada de Trabalhadores** (amber) — agentes, orquestrador, subagents, hierarquia
- **T5 — Camada de Automação** (teal) — hooks, schedules, n8n/Make como linguagens, segurança
- **T6 — Implantação Real** (rose) — 3 casos (Marco/e-commerce, Sally/jurídico, Sana/saúde) + projeto final

### Método com nome próprio

Sugestão principal: **Método PRATO** (apelo brasileiro, conecta com Silver Platter)

- **P** — Preparar os dados
- **R** — Resumir em Silver Platters
- **A** — Agenciar com especialistas
- **T** — Traçar automações e hooks
- **O** — Operar com IA

Alternativas: KISTO, NÚCLEO, DASA, OSIA.

### Projeto final

Aluno termina com um **Agentic OS funcional**:

```
/agentic-os-aluno
  /dados
  /resumos              (Silver Platters)
    financeiro.md
    marketing.md
    operacoes.md
  /skills
  /agentes
    orquestrador.md
    cfo_bot.md
    cmo_bot.md
  /logs
  CLAUDE.md
  plano_30_dias.md
```

Entrega final mínima: relatório semanal automático rodando.

---

## 4. Posicionamento de mercado

### Inimigo

**O improviso com Claude Code.** Não os outros cursos.

### Frase-âncora

> **Enquanto todo mundo ensina Claude Code como ferramenta, eu ensino Claude Code como sistema operacional.**

### Escada de ofertas

1. **Entrada** — Imersão Claude Code (1 dia, surfa a busca)
2. **Principal** — Agentic OS com Claude Code (4 semanas, transformação)
3. **Premium** — Implementação acompanhada (bootcamp/consultoria)

### Antes / Depois

| Antes | Depois |
|---|---|
| Arquivos espalhados | Dados organizados |
| Prompts soltos | Silver Platters |
| Respostas genéricas | CLAUDE.md contextual |
| Agentes sem função | Skills reutilizáveis |
| Retrabalho | Agentes especialistas |
| Medo de automatizar | Orquestrador |
| Zero auditoria | Hooks + logs + segurança |

---

## 5. Estrutura técnica do site

GitHub Pages no formato INEMA.CLUB:

```
agentic-os-curso/
├── index.html                    # Landing page
└── curso/
    ├── trilha1/
    │   ├── index.html
    │   ├── modulo-1-1.html
    │   ├── modulo-1-2.html
    │   └── ...
    ├── trilha2/
    └── ...
```

Identidade visual: dark, neon azul/ciano, painéis holográficos (já validada na imagem "Esqueça a ferramenta. O futuro é o sistema.").

---

## 6. Decisões fechadas com o Nei (rodada 1)

| # | Pergunta | Decisão |
|---|---|---|
| 2 | Público-alvo | **#1 Empreendedores → #2 Consultores → #3 Técnicos** (a copy/tom seguem essa ordem; jovens/devs NÃO são o foco principal) |
| 3 | Escopo de ferramentas | **Foco em Agentic OS** como conceito; Claude Code é a base, Codex e outros agentes também entram como kernel-agnóstico |
| 1, 4–9 | Demais | OK conforme proposto (nome "Agentic OS — O Sistema Operacional do Trabalho com IA", 6 trilhas, método PRATO, INEMA.CLUB, projeto final = Agentic OS funcional + relatório semanal) |

### Implicação da decisão sobre público

A ordem **empreendedor > consultor > técnico** muda a abordagem pedagógica:

- **T1 (Fundamentos)** abre com problema de NEGÓCIO, não com tecnologia. Marco/Sally/Sana entram já na T1, não só na T6.
- Linguagem técnica é progressiva: trilhas iniciais zero código; trilhas finais entram em hooks/MCP.
- Cada módulo abre com "o que isso resolve no seu negócio" antes do "como fazer".
- **Empreendedor pode parar na T4** e já ter valor. Consultor vai até T5. Técnico/builder fecha na T6.

### Implicação da decisão sobre kernel-agnóstico

- **Claude Code** = referência principal (kernel default do curso).
- **Codex** = alternativa para quem está no ecossistema OpenAI.
- **Cursor, Windsurf, Gemini CLI, Kiro** = mencionados como variantes.
- O curso ensina o **CONCEITO**, depois mostra como cada agente implementa.
- Vantagem competitiva: ninguém ensina cross-agent. Todos ensinam "Claude Code do zero".

---

## 7. Análise do `agentic-mk.txt` (atualizado pelo Nei)

Conteúdo: **213 449 chars / 6 287 linhas**. Não é material de marketing — é o **transcript completo do ChatGPT original** + transcrição do vídeo-fonte em inglês (timestamps 00:00 a 22:15).

### Achados que mudam a estratégia

**1. O material-fonte é de um concorrente americano** que já vende:
- Skill `silver-platter` (slash command que mapeia dados em 10–50s, gera HTML com 4 abas)
- "Living Claude Code course" (curso recorrente)
- "Claude Claw business operating system" (produto premium)
- A skill `silver-platter` **já está instalada** no ambiente do Nei (confirmação na lista de skills do Claude Code)

**2. Detalhes técnicos extras que o `agenticOS.txt` deixou de fora**:
- **Pantry / Prep Table / Plate** — metáfora de cozinha pra mapear dados (deve virar uma aula da T3)
- **Interview thorough (30 min) vs fast-track (10 min)** — dois caminhos de implantação
- **HTML output com 4 abas**: audit / data flow / what we'll build / 30-day plan
- **Post-compaction hook** — injeta contexto após compactação (avançado, quase ninguém ensina; vai pra T5)
- **"Skill é jogo infinito"** — princípio pedagógico forte pra T3

**3. Mapa competitivo BR vs US**

| Concorrente (US) | Curso do Nei (BR) |
|---|---|
| Vídeos YouTube + curso "vivo" recorrente | Curso estruturado em 6 trilhas, INEMA.CLUB |
| Foco em Claude Code apenas | Kernel-agnóstico (Claude Code + Codex + outros) |
| Inglês, persona americana (founder-coded) | Português, 3 personas brasileiras |
| Vende skill `silver-platter` pronta | Ensina o aluno a CONSTRUIR a própria silver-platter |
| Sequência: técnico → negócio | Sequência: negócio → consultor → técnico |
| Sem método nomeado | Método **PRATO** (mnemônico BR) |
| Sem governança forte | Governança / auditoria como first-class citizen |
| Sem visão de futuro nomeada | 7 visões de futuro (Personal vs Enterprise OS, memory-as-filesystem, etc.) |

**4. Conclusão**: o material-fonte valida que existe mercado e produto. O Nei tem todos os elementos pra fazer uma versão **mais profunda, mais brasileira e mais arquitetural** — em vez de uma cópia mais rasa.

---

## 8. Validação contra fronteira (pesquisa 2025-2026)

Rodada de pesquisa web confirmou que a tese está **majoritariamente validada** pelo estado-da-arte. Resumo:

### 8.1 Tese validada nos pontos-chave

| Tese | Validação |
|---|---|
| LLMs = "hardware semântico" / nova camada programável | **Karpathy "Software 3.0"** (Sequoia Ascent 2026); Anthropic "context engineering" (set/2025) |
| MCP = "TCP/IP da era agêntica" | **97M downloads mensais em mar/2026**; adoção OpenAI (mar/2025), Google (abr/2025), Microsoft, Salesforce; governança sob Linux Foundation desde dez/2025 |
| Hooks = "interrupts" do OS agêntico | Documentação oficial Anthropic confirma comportamento determinístico (PreToolUse pode bloquear, Stop com exit 2 força continuação) |
| Orquestração hierárquica > plana | Anthropic mediu **90,2% de melhora** com Opus 4 lead + Sonnet 4 workers; LangGraph/CrewAI/AutoGen/OpenAI Agents SDK convergiram pro mesmo pattern |
| Memória = novo filesystem | **Letta/MemGPT** (UC Berkeley) implementa literalmente — core memory = RAM, archival = disk; Karpathy "LLM Wiki pattern"; Claude Code 3-level memory |
| AGENTS.md como identidade de agente | **Padrão multi-vendor** sob Linux Foundation — usado por OpenAI Codex, Google Jules, Amp, Cursor, Factory; site oficial em [agents.md](https://agents.md/) |
| Compute substitutivo, não aditivo | Consenso de Karpathy + Masad (Replit) + a16z + Sequoia em 2026 |

### 8.2 CLI como "shell do Agentic OS" — ponto adicional do Nei

Insight crítico que a pesquisa não tinha capturado: **a CLI virou o shell padrão para trabalho agêntico sério**. Consolidação tão forte quanto o MCP:

- **Claude Code** (Anthropic), **Codex CLI** (OpenAI), **Gemini CLI** (Google), **Cursor CLI**, **Aider**, **Continue.dev**, **Replit Agent** — todos CLI-first em 2025-2026.

**Por que a CLI venceu**:
1. Composabilidade com shell, pipes, cron
2. Git-nativo (worktrees, branches, commits)
3. Acesso direto ao filesystem (sem sandbox)
4. Hooks e automação triviais
5. Roda em servidor remoto / SSH
6. Paralelização de sessões
7. Baixa latência, sem overhead de UI

**Mapeamento atualizado das camadas**:

| Era clássica | Era agêntica |
|---|---|
| Hardware (CPU/RAM/disco) | LLMs (Claude, GPT, Gemini) |
| Kernel / SO | **Agentic OS** (CLAUDE.md, skills, hooks, orquestrador) |
| **Shell (bash, zsh)** | **CLI agêntica** (Claude Code, Codex CLI, Gemini CLI) ← **adição** |
| Protocolos (TCP/IP, POSIX) | **MCP** + **A2A** (Google Agent2Agent) |
| Linguagens (C, Python) | n8n, Make, LangGraph, Python+SDK |
| Aplicações (Word, Photoshop) | Agentes especializados |
| Sistema de arquivos | Silver Platters + RAG + memory blocks (Letta) |
| Interrupts (timer, I/O) | Hooks (SessionStart, PostToolUse, Stop) |

### 8.3 Gaps na tese — o que precisa entrar no curso pra ele ficar "à frente"

Seis pontos que a pesquisa identificou como ausentes na tese e que precisam virar conteúdo:

1. **A2A (Google Agent2Agent)** — protocolo de segunda camada. MCP conecta agente↔ferramenta; A2A conecta agente↔agente. Stack completo = MCP + A2A. Mais de 150 parceiros, 22k+ stars no GitHub em abr/2026.

2. **Context Engineering como disciplina própria** — Anthropic publicou em set/2025 como conceito distinto de prompt engineering. Não é "prompt para agentes", é a engenharia de qual configuração de contexto produz o comportamento desejado. Merece módulo próprio na T3.

3. **Computer Use / Browser Agents como camada** — Anthropic Computer Use, OpenAI Operator, Perplexity Comet, OpenAI Atlas. Mercado vai de US$4,5B (2024) → US$76,8B (2034). Agentes que operam pixels, não só APIs. Categoria T5 ou T6.

4. **Observabilidade / avaliação de agentes** — LangSmith, Letta Evals, Claude traces, Anthropic "Measuring AI agent autonomy in practice". Sem isso, não há governança real. Deve ser parte da T5.

5. **Managed Agents como "cloud OS"** — Anthropic lançou Managed Agents em abr/2026 (US$0,08/session-hour). Modelo de hosting de agente como serviço. Tópico avançado pra T6.

6. **"Jagged Intelligence" (Karpathy)** — framework pedagógico crucial. Agentes podem refatorar 100k linhas de código mas falham em raciocínios triviais. Saber **onde delegar e onde não delegar** é tão importante quanto saber como. Vai na T1 (fundamentos).

### 8.4 Cenário brasileiro — gap competitivo confirmado

Pesquisa confirmou: **nenhum curso BR opera no nível de abstração de OS aplicado a agentes** com terminologia alinhada a 2025-2026.

- RocketSeat (pós em IA/Automação) — foco em automação, não em arquitetura agêntica
- Alura — introdutório/intermediário, sem Agentic OS como framework
- Filipe Deschamps / curso.dev — dev generativo, não arquitetura agente
- NoCode Startup, Imersão Builder — Claude Code como ferramenta, sem visão de OS

**Espaço para ser a primeira referência brasileira de Agentic OS como disciplina de engenharia.** Alinhado ao funil: curso público (autoridade) → comunidade inema.vip → imersão high-ticket.

### 8.5 Estado do repo GitHub

`https://github.com/inematds/agenticos` — **repo vazio** (só tem `.git`, nenhum commit). Começamos do zero, sem legado a preservar.

---

## 9. Estrutura do curso — versão refinada após pesquisa

As 6 trilhas mantidas, agora com os gaps incorporados:

| Trilha | Cor INEMA | Conteúdo refinado |
|---|---|---|
| **T1 — Fundamentos do Agentic OS** | emerald | Tese das camadas (com CLI = shell), Software 3.0 (Karpathy), jagged intelligence, 3 personas (Marco/Sally/Sana) já como ganchos |
| **T2 — Camada de Identidade** | blue | CLAUDE.md, AGENTS.md (padrão multi-vendor), regras de escopo, governança como first-class citizen |
| **T3 — Camada de Conhecimento** | purple | Silver Platters, Context Engineering (Anthropic), Pantry/Prep/Plate, Skills (Claude + Codex), MCP, memory blocks (Letta) |
| **T4 — Camada de Trabalhadores** | amber | Orchestrator-Workers (Anthropic 90,2%), subagents, A2A, chief-of-staff pattern, exemplos cross-framework (LangGraph/CrewAI) |
| **T5 — Camada de Automação e Observabilidade** | teal | Hooks como interrupts, n8n/Make como linguagens complementares, Computer Use / browser agents, avaliação e tracing |
| **T6 — Implantação Real** | rose | 3 casos completos (e-commerce, jurídico, saúde), Managed Agents, projeto final = Agentic OS funcional + relatório semanal |

---

## 10. Próximos passos

1. ~~Nei responde as 10 perguntas~~ ✅ rodada 1 fechada
2. ~~Pesquisa de validação contra fronteira~~ ✅ feita; tese validada + 6 gaps + insight da CLI
3. ~~Estado do repo GitHub~~ ✅ vazio, começamos do zero
4. **(próximo)** Claude monta esqueleto:
   - `index.html` (landing)
   - 6 `curso/trilhaN/index.html` (índices de trilha)
   - 1 módulo-piloto: `curso/trilha1/modulo-1-1.html` (Fundamentos — A tese das camadas)
5. Nei valida o módulo-piloto
6. Claude produz os ~36 módulos restantes (6 trilhas × 6 módulos mínimo) seguindo o padrão validado
7. Publicação no GitHub Pages (repo `inematds/agenticos`)
8. (Pendente) Definir domínio próprio ou usar `inematds.github.io/agenticos`

---

## 11. Fontes da pesquisa (selecionadas)

- [Karpathy — Sequoia Ascent 2026 (Software 3.0, Agentic Engineering)](https://karpathy.bearblog.dev/sequoia-ascent-2026/)
- [Anthropic — Building Effective Agents (dez/2024)](https://www.anthropic.com/research/building-effective-agents)
- [Anthropic — Effective Context Engineering (set/2025)](https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents)
- [Anthropic — Multi-agent Research System (jun/2025)](https://www.anthropic.com/engineering/multi-agent-research-system)
- [Claude Code Hooks Docs](https://docs.anthropic.com/en/docs/claude-code/hooks)
- [Claude Code Memory Docs](https://docs.anthropic.com/en/docs/claude-code/memory)
- [Claude Code Skills Docs](https://docs.anthropic.com/en/docs/claude-code/skills)
- [MCP — Model Context Protocol](https://modelcontextprotocol.io/introduction)
- [Google A2A — Agent2Agent Protocol](https://developers.googleblog.com/en/a2a-a-new-era-of-agent-interoperability/)
- [AGENTS.md — padrão multi-vendor](https://agents.md/)
- [OpenAI Codex AGENTS.md](https://developers.openai.com/codex/guides/agents-md)
- [Letta — Agent Memory blog](https://www.letta.com/blog/agent-memory)
- [Letta — Letta Code (mar/2026)](https://www.letta.com/blog/letta-code)
- [Martin Fowler — Context Engineering for Coding Agents](https://martinfowler.com/articles/exploring-gen-ai/context-engineering-coding-agents.html)
- [A16Z — Trillion Dollar AI Software Development Stack](https://a16z.com/the-trillion-dollar-ai-software-development-stack/)
- [Sequoia AI 50 2025](https://sequoiacap.com/article/ai-50-2025/)
- [AgenticOS Workshop ASPLOS 2026](https://os-for-agent.github.io/)
- [Pento — A Year of MCP: 2025 Review](https://www.pento.ai/blog/a-year-of-mcp-2025-review)

---

## 7. Próximos passos sugeridos

1. Nei responde as 10 perguntas (texto livre)
2. Claude monta esqueleto: landing + 6 índices de trilha + 1 módulo-piloto da T1
3. Nei valida o módulo-piloto
4. Claude produz os 30+ módulos restantes seguindo o padrão validado
5. Publicação no GitHub Pages

---

## Fontes do conteúdo

- `/home/nmaldaner/projetos/agenticos/doc/agenticOS.txt` (70k chars, transcrição completa da sessão original)
- Imagens em `/home/nmaldaner/projetos/agenticos/doc/*.png` (identidade visual neon futurista)
- Skill `formato-curso` (INEMA.CLUB design system)
- Pesquisa de mercado BR (Udemy, Hotmart, Sympla, NoCode Startup, Imersão Builder, Claude Academy)
