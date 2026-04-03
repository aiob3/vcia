# WORKFLOW — VCIA

## Visão geral do processo

```
Exploração visual → Onboarding canônico → Blueprint → IDE agêntica → Implementação
```

O workflow separa deliberadamente a fase de fechamento de ideia da fase de implementação. Nenhuma linha de código é escrita antes que os contratos mínimos de onboarding estejam versionados.

## Fases

### Phase 0 — Fechamento da ideia ✅

**Objetivo:** consolidar entendimento antes de qualquer implementação.

**Entregáveis:**
- Statement do projeto em 1 parágrafo
- Escopo inicial definido
- Referências aproveitadas e descartadas identificadas

**Gate de saída:** o projeto consegue ser explicado sem citar a referência como muleta conceitual.

**Status:** concluído — referência SetupVibe extraída, workflow neutro definido, identidade própria em andamento.

---

### Phase 1 — Onboarding canônico 🔄

**Objetivo:** criar o kit mínimo versionado no GitHub como base de alinhamento para toda a equipe e agentes.

**Entregáveis:**
- `README.md`
- `PROJECT_SCOPE.md`
- `WORKFLOW.md`
- `DECISION_LOG.md`
- `AGENT_ONBOARDING.md`

**Gate de saída:** uma pessoa externa entende o projeto, o momento atual e os próximos passos apenas lendo os arquivos-base. Nenhum arquivo contém TODOs sem dono ou data.

---

### Phase 2 — Blueprint do produto ⏳

**Objetivo:** quebrar a visão em blocos operacionais para handoff à IDE.

**Entregáveis:**
- Sitemap de páginas e superfícies
- Lista de componentes e módulos
- Fluxo principal do usuário
- Backlog inicial por épicos
- Matriz de dependências (front / script / docs / automação)

**Gate de saída:** o agente de desenvolvimento pode iniciar implementação por fases sem contexto oral adicional.

---

### Phase 3 — Escritório agêntico na IDE ⏳

**Objetivo:** iniciar o projeto em ambiente de desenvolvimento com responsabilidades explícitas por agente.

**Entregáveis:**
- Estrutura inicial do repositório de implementação
- Prompt base de instrução para agentes
- Sequência de execução por fase
- Regras de integração, validação e versionamento

**Gate de saída:** cada agente sabe o que recebe, o que entrega e quando precisa escalar dúvida ao operador.

---

### Phase 4 — Implementação controlada ⏳

**Objetivo:** construir a primeira versão funcional sem descaracterizar o workflow base.

**Entregáveis:**
- Landing page funcional
- Documentação técnica mínima
- Script de instalação (ou placeholder validado)
- Validação do fluxo fim a fim

**Gate de saída:** o projeto demonstra a tese principal de onboarding, mesmo com stack ainda incompleta.

## Trilhas paralelas

Trabalhos que ocorrem em paralelo e só são integrados depois de validados:

| Trilha | Objetivo | Condição para integrar |
|---|---|---|
| Naming e posicionamento | Identidade própria do projeto | Nome, promessa e escopo aprovados pelo operador |
| Arquitetura de conteúdo | Mapa de páginas e documentos | Estrutura navegável validada |
| Stack real | Ferramentas, runtimes e scripts | Dependências mínimas definidas |
| Protocolo de agentes | Papéis, entradas e saídas | Responsabilidades sem sobreposição |
| Critérios de readiness | Checklist de prontidão para IDE | Todos os mínimos presentes |

## Regras do workflow

- Nenhuma fase começa sem que o gate da fase anterior tenha sido aprovado pelo operador
- Decisões abertas são registradas em `DECISION_LOG.md` antes de prosseguir
- Artefatos de trilhas paralelas só entram no tronco principal após validação explícita
- O operador é consultado sempre que uma lacuna impactar mais de uma fase
