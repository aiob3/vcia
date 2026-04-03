# AGENT_ONBOARDING — VCIA

## Para quem é este documento

Este documento é o ponto de entrada obrigatório para qualquer agente de desenvolvimento que for atuar neste projeto. Ele define o contexto, as responsabilidades, os contratos de trabalho e o protocolo de escalonamento.

Leia antes de executar qualquer tarefa.

## Contexto do projeto

VCIA é um workflow base para inicialização de projetos de desenvolvimento com IA. O objetivo é criar um template canônico replicável — não um produto acabado neste momento.

O projeto está na transição entre Phase 1 (onboarding) e Phase 2 (blueprint). Nenhuma implementação de front ou script deve ser iniciada antes que o gate da Phase 2 seja aprovado pelo operador.

## Referência estrutural

O modelo de referência é o site [SetupVibe](https://setupvibe.dev/), usado apenas como ponto de partida estrutural. O projeto VCIA não é um clone do SetupVibe. A referência informa a arquitetura de páginas e a lógica de onboarding técnico, mas a identidade, copy e stack serão próprias.

## Cadeia de responsabilidade

| Papel | Responsabilidade |
|---|---|
| Operador | Visão, aprovação de gates, decisões abertas (DECISION_LOG) |
| Agente de planejamento (Perplexity) | Exploração, síntese, estruturação de onboarding e briefings |
| Agente de desenvolvimento (IDE) | Implementação de phases, geração de código, validação técnica |
| Agente de revisão | QA de entregáveis, checagem de critérios de aceitação |

## Contratos de trabalho por agente

### Agente de desenvolvimento

**Recebe:**
- Fase ativa com `phase_id`, `objective`, `tasks` e `definition_of_done`
- DECISION_LOG atualizado com pendências conhecidas
- Arquivos de contexto relevantes da pasta `docs/`

**Entrega:**
- Artefatos especificados nos entregáveis da fase
- Registro de novas lacunas encontradas durante execução
- Pull Request com descrição referenciando `phase_id` e tasks executadas

**Não faz sem aprovação do operador:**
- Avançar para a próxima fase sem gate aprovado
- Tomar decisões de D001–D005 por conta própria
- Criar componentes fora do escopo da fase ativa

## Protocolo de lacunas e decisões

Quando encontrar uma lacuna, bifurcação ou decisão não registrada:

1. **Não bloqueie a execução** — continue com as tasks que não dependem da lacuna
2. **Registre a lacuna** — adicione entry em `DECISION_LOG.md` com status ABERTO
3. **Ofereça 2-3 hipóteses** — informe ao operador as opções com impacto de cada uma
4. **Aguarde confirmação** — antes de integrar qualquer solução para a lacuna no tronco principal

Se a lacuna bloquear totalmente a tarefa em andamento, finalize o que for possível e sinalize claramente qual decision_id está impedindo o avanço.

## Convenções de commit

```
[phase_id] tipo: descrição curta

Exemplos:
[p1] docs: adiciona PROJECT_SCOPE.md
[p2] feat: blueprint de superfícies e sitemap
[p3] chore: estrutura base do repositório de implementação
[p4] feat: landing page hero inicial
```

Tipos válidos: `feat`, `fix`, `docs`, `chore`, `refactor`, `test`

## Checklist de prontidão para Phase 3

Antes de abrir a IDE e iniciar o escritório agêntico, verifique:

- [ ] `README.md` está versionado e legível por agente externo
- [ ] `PROJECT_SCOPE.md` define escopo e exclusões sem ambiguidade
- [ ] `WORKFLOW.md` tem fases, gates e trilhas paralelas documentadas
- [ ] `DECISION_LOG.md` tem todas as pendências conhecidas registradas
- [ ] `AGENT_ONBOARDING.md` (este arquivo) está completo e acessível
- [ ] D001 (naming) está pelo menos em análise com documento paralelo criado
- [ ] D004 (ambiente de implementação) está decidido
- [ ] O operador aprovou o gate da Phase 1

## Regras gerais

- KISS: faça a solução mais simples que satisfaz o critério de aceitação
- DRY: nunca duplique informação que já existe em outro arquivo deste repo
- YAGNI: não implemente o que está fora do escopo da fase ativa
- Toda ambiguidade deve virar uma entrada em `DECISION_LOG.md`, não uma suposição silenciosa
