# Onboarding do Projeto — Workflow Base para Novo Setup

## Objetivo

Este documento formaliza o onboarding de um novo projeto a partir de um workflow-base reutilizável, inspirado em referências como o SetupVibe, mas deliberadamente desacoplado da semântica, branding e limitações do modelo original.[page:1][page:2][page:3][page:4]

O propósito é transformar conhecimento tácito já dominado pelo operador em uma estrutura explícita, rastreável e reutilizável, adequada para ser incorporada em repositório GitHub e depois operacionalizada na IDE por agentes responsáveis pela implementação em fases.[cite:2][cite:3][cite:12]

## Premissa de trabalho

O processo assume que a etapa atual não é ainda a implementação final do produto, mas o fechamento da ideia e a consolidação de um artefato de onboarding que sirva como ponto de partida para a equipe de projeto e para o escritório agêntico a ser iniciado na IDE.[cite:2][cite:12]

Nesse contexto, a função desta etapa é servir como camada de tradução entre visão estratégica, exploração visual e execução técnica, de forma que o projeto comece com menos ambiguidade e menor dependência de contexto implícito do operador.[cite:3][cite:10]

## O que está claro e válido

- A intenção de usar uma referência externa apenas como ponto de partida estrutural é válida, porque permite acelerar descoberta sem aprisionar o projeto à narrativa do modelo original.[page:1][page:2]
- A decisão de tratar o onboarding como uma etapa própria do projeto é correta, porque separa exploração, definição e execução em camadas mais governáveis.[cite:2][cite:3]
- A ideia de fechar a visão antes de abrir a IDE é especialmente coerente com um processo iterativo orientado por prototipagem e contratos mínimos de trabalho.[cite:2][cite:10]
- O uso de fases, gates e lacunas como objetos explícitos melhora a transferibilidade para agentes de desenvolvimento e reduz retrabalho posterior.[cite:10][cite:14]

## O ajuste mais importante

O principal ajuste necessário não é de direção, mas de formalização: o projeto precisa de um artefato canônico que separe claramente referência, workflow genérico e instância específica do projeto.[page:1][cite:10]

Sem essa separação, a equipe ou os agentes de IDE podem confundir o que deve ser copiado, o que deve ser reinterpretado e o que já pertence à identidade própria do novo projeto.[cite:3][cite:12]

## Modelo de camadas

### Camada 1 — Referência observada

Define o que foi extraído da referência externa e por que isso importa.

- Estrutura de navegação.[page:1]
- Tipos de páginas e objetivos de cada uma.[page:1][page:2][page:3][page:4]
- Padrões de copy, CTA, prova, compatibilidade e organização visual.[page:1]
- Estratégia de conversão entre descoberta, entendimento técnico e instalação.[page:1][page:2][page:4]

### Camada 2 — Workflow genérico

Transforma a referência em um método reutilizável para qualquer novo projeto de setup, onboarding técnico ou plataforma de inicialização.[cite:2][cite:10]

- Quais fases sempre existem.
- Quais decisões dependem do operador.
- Quais artefatos precisam existir antes da implementação.
- Quais lacunas devem ser mitigadas em paralelo antes da integração no tronco principal do projeto.

### Camada 3 — Instância do projeto atual

Define a identidade própria do projeto que será criado no repositório.

- Nome e semântica próprios.
- Stack real desejada.
- Escopo inicial válido.
- Diferenças em relação ao modelo de referência.
- Critérios de aceitação para primeira entrega.

## Estrutura operacional recomendada

### Phase 0 — Fechamento da ideia

**Objetivo:** consolidar o entendimento do que está sendo criado antes de qualquer implementação.

**Entregáveis:**
- Statement do projeto em 1 parágrafo.
- Escopo inicial em 5 a 10 bullets.
- O que o projeto é.
- O que o projeto não é.
- Lista de referências aproveitadas e descartadas.

**Gate:** o projeto consegue ser explicado sem citar o SetupVibe como muleta conceitual.[page:1][page:2]

### Phase 1 — Documento de onboarding

**Objetivo:** criar o artefato que será versionado no GitHub como base de alinhamento.

**Entregáveis:**
- `README` orientado a visão.
- `PROJECT_SCOPE.md` com objetivo, escopo, exclusões e critérios.
- `WORKFLOW.md` com fases, gates e papéis.
- `DECISION_LOG.md` para registrar escolhas e pendências.
- `PARALLEL_TRACKS.md` para atividades que precisam ser mitigadas antes de integrar.

**Gate:** uma pessoa externa consegue entender o projeto, o momento atual e os próximos passos apenas lendo os arquivos-base.[cite:12][cite:14]

### Phase 2 — Blueprint do produto

**Objetivo:** quebrar a visão em blocos operacionais para handoff à IDE.

**Entregáveis:**
- Sitemap ou mapa de superfícies.
- Lista de componentes e módulos.
- Fluxo principal do usuário.
- Backlog inicial por épicos.
- Matriz de dependências entre front, script, docs e automação.

**Gate:** o agente de desenvolvimento consegue iniciar implementação por fases sem depender de contexto oral adicional.[cite:10][cite:12]

### Phase 3 — Escritório agêntico na IDE

**Objetivo:** iniciar o projeto em ambiente de desenvolvimento com responsabilidades explícitas para cada agente.

**Entregáveis:**
- Estrutura inicial do repositório.
- Prompt/base de instruções para agentes.
- Sequência de execução por fase.
- Regras de integração, validação e versionamento.

**Gate:** cada agente sabe o que recebe, o que entrega e quando precisa escalar dúvida ao operador.[cite:3][cite:12]

### Phase 4 — Implementação controlada

**Objetivo:** construir a primeira versão funcional sem descaracterizar o workflow-base.

**Entregáveis:**
- Front inicial.
- Documentação técnica mínima.
- Scripts ou placeholders de instalação.
- Primeira validação do fluxo fim a fim.

**Gate:** o projeto já demonstra a tese principal de onboarding, mesmo que a stack final ainda esteja incompleta.[cite:2][cite:10]

## Marcos decisórios

Os pontos de dúvida e lacuna não devem aparecer apenas como observações soltas. Eles precisam existir como marcos decisórios com contexto, impacto e ação paralela obrigatória.[cite:3][cite:10]

### Marco 1 — Quanto da referência será herdado

**Pergunta:** o novo projeto herda apenas a arquitetura informacional ou também parte da lógica de setup e da copy de ativação?[page:1][page:2][page:3]

**Risco se não decidir:** o projeto pode nascer como clone disfarçado, sem diferenciação real.

**Atividade paralela de mitigação:** criar tabela “copiar / reinterpretar / descartar” para cada elemento extraído da referência.[page:1][page:2][page:3][page:4]

### Marco 2 — Qual é o escopo do onboarding

**Pergunta:** o onboarding cobre apenas a entrada no projeto, ou já define também a lógica padrão de operação dos agentes dentro da IDE?[cite:12]

**Risco se não decidir:** o repositório mistura documentação institucional com protocolo operacional interno.

**Atividade paralela de mitigação:** separar documentos de visão, execução e governança dos agentes.

### Marco 3 — O que precisa existir antes de codar

**Pergunta:** quais artefatos são pré-requisitos obrigatórios para abrir a IDE com segurança operacional?[cite:2][cite:10]

**Risco se não decidir:** a IDE vira espaço de descoberta improvisada, e não de execução.

**Atividade paralela de mitigação:** checklist de readiness com arquivos mínimos, backlog e decisões pendentes.

### Marco 4 — Qual será a identidade própria do projeto

**Pergunta:** qual narrativa, semântica e proposta substituem definitivamente a visão emprestada da referência?[page:1][page:2]

**Risco se não decidir:** o projeto começa funcionalmente, mas sem tese própria e sem consistência de naming.

**Atividade paralela de mitigação:** documento de posicionamento com nome, promessa, público e diferenciação.

## Trilhas paralelas antes da integração

Alguns trabalhos devem ocorrer em paralelo e só depois serem integrados como parte oficial da estrutura do projeto.

| Trilha | Objetivo | Saída esperada | Condição para integrar |
|---|---|---|---|
| Naming e posicionamento | Definir identidade própria do projeto | Documento de posicionamento | Nome, promessa e escopo aprovados |
| Arquitetura de conteúdo | Separar landing, docs, install e workflow | Sitemap e mapa de documentos | Estrutura navegável validada |
| Stack real | Traduzir visão para stack efetiva | Matriz de ferramentas, runtimes e scripts | Dependências mínimas definidas |
| Protocolo de agentes | Definir papéis, entradas, saídas e escalonamento | Guia operacional por agente | Responsabilidades sem sobreposição |
| Critérios de readiness | Garantir que a IDE abra com base sólida | Checklist de prontidão | Todos os mínimos obrigatórios presentes |

## Estrutura sugerida para o repositório

```text
repo/
├─ README.md
├─ PROJECT_SCOPE.md
├─ WORKFLOW.md
├─ DECISION_LOG.md
├─ PARALLEL_TRACKS.md
├─ AGENT_ONBOARDING.md
├─ docs/
│  ├─ reference-extraction.md
│  ├─ product-blueprint.md
│  ├─ architecture-map.md
│  └─ naming-positioning.md
├─ prompts/
│  ├─ ide-agent-system.md
│  ├─ dev-agent-phase-01.md
│  ├─ dev-agent-phase-02.md
│  └─ reviewer-agent.md
└─ project/
   └─ implementation-base/
```

Essa estrutura favorece a separação entre visão, decisão, execução e artefatos operacionais, o que conversa bem com seu uso de GitHub como ponto de sincronização e posterior execução em IDE conectada a fluxo agentic.[cite:12]

## Como o onboarding deve mudar neste projeto

A mudança mais importante neste projeto é que o onboarding não deve nascer como simples documento de recepção, e sim como mecanismo de fechamento de contexto antes da abertura do ambiente de execução.[cite:2][cite:3]

Em vez de “abrir repo e começar a fazer”, a nova lógica fica assim:

1. Explorar a referência visual e estrutural.
2. Traduzir para workflow neutro.
3. Fechar identidade e escopo do projeto.
4. Registrar os artefatos-base no GitHub.
5. Só então abrir a IDE e iniciar o escritório agêntico.

Essa inversão é valiosa porque protege a fase de implementação contra ambiguidade estrutural e reduz o risco de o projeto ser guiado pela ferramenta em vez de ser guiado pela intenção do operador.[cite:2][cite:12]

## Protocolo para o agente de desenvolvimento

Ao entregar para o agente no IDE, o onboarding deve ser consumível em blocos pequenos, objetivos e verificáveis.[cite:10][cite:14]

Cada phase deve conter:
- `phase_id`
- `phase_name`
- `objective`
- `inputs`
- `tasks`
- `outputs`
- `open_questions`
- `parallel_dependencies`
- `definition_of_done`

Esse formato reduz interpretação excessiva e facilita versionamento incremental do projeto.[cite:10][cite:14]

## Recomendação prática imediata

O próximo movimento mais efetivo não é abrir a IDE ainda. O próximo movimento é abrir o repositório e versionar o kit mínimo de onboarding do projeto.[cite:2][cite:12]

O kit mínimo recomendado é:
- `README.md`
- `PROJECT_SCOPE.md`
- `WORKFLOW.md`
- `DECISION_LOG.md`
- `AGENT_ONBOARDING.md`

Com isso, a abertura da IDE já acontece com fronteiras de execução mais claras, e o escritório agêntico nasce com contexto suficiente para trabalhar em fases sem depender de reconstrução constante da intenção original.[cite:3][cite:12]

## Decisão sugerida para agora

A direção está clara e é efetiva. O ajuste necessário é operacional: converter a visão em um pacote canônico de onboarding de repositório antes de iniciar a implementação.[cite:2][cite:3]

O caminho mais sólido para este projeto é:
- fechar a estrutura canônica de onboarding;
- publicar essa base no GitHub;
- abrir a IDE com phases e gates já definidos;
- só então iniciar a construção do projeto.

Esse desenho é compatível com a forma como o operador já vem trabalhando em paralelo e cria uma ponte limpa entre exploração visual, documentação estratégica e execução técnica assistida por agentes.[cite:2][cite:3][cite:12]
