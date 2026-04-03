# VCIA

> Workflow base para setup de ambiente de desenvolvimento com IA — ponto de partida replicável para qualquer novo projeto.

## O que é este projeto

VCIA é um workflow estruturado para inicialização de ambientes de desenvolvimento orientados a IA. Funciona como template canônico de onboarding: você abre um repositório, preenche os contratos mínimos, e a equipe de agentes já tem contexto suficiente para executar em fases.

Não é um produto final. É a infraestrutura de projeto que evita improvisar contexto na IDE.

## O que este projeto não é

- Não é um clone do SetupVibe (usado apenas como referência estrutural de partida)
- Não é um script de instalação pronto
- Não é documentação de produto acabado
- Não é um template genérico de landing page

## Status atual

| Phase | Nome | Status |
|---|---|---|
| Phase 0 | Fechamento da ideia | ✅ Concluído |
| Phase 1 | Onboarding canônico (este repo) | 🔄 Em andamento |
| Phase 2 | Blueprint do produto | ⏳ Pendente |
| Phase 3 | Escritório agêntico na IDE | ⏳ Pendente |
| Phase 4 | Implementação controlada | ⏳ Pendente |

## Estrutura do repositório

```text
vcia/
├─ README.md                  ← visão geral e status
├─ PROJECT_SCOPE.md           ← objetivo, escopo, exclusões, critérios
├─ WORKFLOW.md                ← fases, gates e definições de pronto
├─ DECISION_LOG.md            ← registro de escolhas e pendências
├─ AGENT_ONBOARDING.md        ← protocolo para agentes na IDE
├─ docs/
│  ├─ reference-extraction.md ← extração do modelo SetupVibe
│  ├─ product-blueprint.md    ← mapa de superfícies e componentes
│  └─ naming-positioning.md   ← identidade e diferenciação
├─ prompts/
│  ├─ ide-agent-system.md     ← instruções base para agentes
│  └─ phase-agents/           ← instruções específicas por fase
└─ project/
   └─ implementation-base/    ← código e artefatos de implementação
```

## Como usar este template

1. Leia `PROJECT_SCOPE.md` para entender o que está sendo construído
2. Leia `WORKFLOW.md` para entender as fases e os gates
3. Consulte `DECISION_LOG.md` para ver pendências abertas
4. Se você é um agente de desenvolvimento, comece por `AGENT_ONBOARDING.md`

## Referências

- Referência estrutural: [SetupVibe](https://setupvibe.dev/)
- Organização: [aiob3](https://github.com/aiob3)
