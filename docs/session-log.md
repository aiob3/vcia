# session-log.md
> Racional consolidado das sessões de onboarding do projeto VCIA
> #ID 030426-164900 | racional fechado

---

## Resumo executivo

Este documento fecha o ciclo de onboarding iniciado em 03/04/2026. Registra o que foi tratado, as decisões tomadas, as pendências abertas e o veredito sobre o próximo passo: **IDE agora ou iterar mais**.

**Veredito: IR PARA A IDE AGORA.** Todos os bloqueadores de Phase 3 são de Fase posterior (Phase 4). A prototipagem estrutural e narrativa no Replit pode começar imediatamente com placeholders.

---

## Linha do tempo das interações

### Interação 1 — Extração SetupVibe
**#ID 030426-152700**

**O que foi feito:**
- Mapeamento completo das 4 superfícies do site SetupVibe (home, como funciona, ferramentas, instalar)
- Identificação dos 9 blocos da home com função de cada um
- Catalogação da stack técnica por categoria (shell, AI CLI, runtimes, DevOps, CLI moderno, infra)
- Mapeamento de padrões de copy, CTA e prova social
- Identificação das lacunas que precisam ser validadas antes de copiar 1:1

**Decisão tomada:** SetupVibe como referência estrutural, não template. Foco no pipeline de provisionamento, não só no front-end.

---

### Interação 2 — Estrutura de onboarding e workflow
**#ID 030426-153540 / 030426-154300**

**O que foi feito:**
- Validação de que a abordagem "workflow base + fases + gates" é coerente com o estilo de trabalho do operador (KTX, templates, prototipagem antes de MVP)
- Definição do modelo de 3 camadas: referência observada → workflow genérico → instância do projeto
- Estruturação do workflow em 5 phases (0 a 4) com gates HITL explícitos
- Identificação de 4 marcos decisórios com atividades paralelas obrigatórias
- Definição da estrutura do repositório: README, PROJECT_SCOPE, WORKFLOW, DECISION_LOG, AGENT_ONBOARDING + docs/ + prompts/
- Estabelecimento do fluxo canônico: **fechar ideia → versionar no GitHub → abrir IDE → escritório agêntico**

**Decisão tomada:** onboarding é mecanismo de fechamento de contexto, não boas-vindas.

---

### Interação 3 — Frameworks, skills e studies mapeados
**#ID 030426-163700**

**O que foi ingerido:**

| Fonte | Papel no projeto |
|-------|------------------|
| aiob3/aicod071 | Framework central PREVC, padrão .context/ universal |
| gsd-build/get-shit-done | Workflow engine, docs pt-BR |
| docker/docker-agent | Skill base para orquestração de containers |
| NousResearch/hermes-agent | Template de agent com raciocínio estruturado |
| NousResearch/hermes-agent-self-evolution | Loop de auto-evolução via feedback |
| NousResearch/hermes-paperclip-adapter | Bridge Hermes ↔ Paperclip |
| paperclipai/paperclip | Context protocol entre agentes |
| Anthropic Harness Design | Padrão de harness para sessões longas |
| chroma-core/context-rot | Estratégia anti-degradação de contexto |
| aiob3/chunkit | Fragmentação inteligente para LLMs |
| aiob3/llm-readable-kit | Formatação de docs para máxima legibilidade por LLMs |

**Decisão tomada:** toda documentação do projeto será gerada com padrões do llm-readable-kit e fragmentada via chunkit antes de ser ingerida por agentes em sessões longas.

---

### Interação 4 — Push no repositório aiob3/vcia
**#ID 030426-164300**

**O que foi feito:**
- Repositório aiob3/vcia identificado (já existia com 6 arquivos base)
- Push de estrutura completa: docs/, prompts/, phase-agents/
- AGENT_ONBOARDING.md enriquecido com toda a cadeia de frameworks
- Este session-log criado como fechamento formal do ciclo de onboarding

---

## Estado atual das decisões

| ID | Decisão | Status | Ação para desbloquear |
|----|---------|--------|------------------------|
| D001 | Naming e identidade própria | ABERTO | Preencher `docs/naming-positioning.md` |
| D002 | Escopo real do script de setup | ABERTO | Levantar stack real do operador |
| D003 | Quanto da copy do SetupVibe reutilizar | ABERTO | Usar tabela em `docs/reference-extraction.md` |
| D004 | Ambiente de implementação (Replit/local/Codespaces) | **DECIDIDO** | Replit para prototipagem inicial |
| D005 | Protocolo de escalonamento dos agentes | **DECIDIDO** | Documentado em `AGENT_ONBOARDING.md` e `prompts/ide-agent-system.md` |

---

## Análise: Partir para IDE ou Iterar?

| Critério | Estado | Bloqueia Phase 3? |
|----------|--------|-------------------|
| Racional documentado | ✅ Completo | Não |
| Blocos da home mapeados | ✅ 9 blocos mapeados | Não |
| AGENT_ONBOARDING pronto | ✅ Completo | Não |
| D004 ambiente decidido | ✅ Replit | Não |
| D005 protocolo de agentes | ✅ Definido | Não |
| Stack real definida | ⏳ Placeholder | Não (só Phase 4) |
| Identidade visual definida | ⏳ Placeholder | Não (só Phase 4) |
| Comando de install testado | ⏳ Pendente | Não (só Phase 4) |
| D001 naming resolvido | ⏳ Em análise | Não (só Phase 4) |

**Conclusão:** todos os itens pendentes são de Phase 4, não de Phase 3. A prototipagem estrutural e narrativa no Replit pode começar agora com placeholders. O prototype com placeholder É o ponto de validação antes de trazer os dados reais.

---

## Próximos passos (sequência exata)

### Agora — Abrir IDE (Phase 3)
1. Abrir Replit
2. Apontar para https://github.com/aiob3/vcia
3. Rodar: `npx @ai-coders/context mcp:install`
4. Colar no agente:
```
init the context
```
```
plan [vcia landing page base - fase 1: home + instalar] using ai-context
```
```
start the workflow
```
5. O agente lê `prompts/phase-agents/phase-01-landing.md` e executa as 10 tasks da home

### Em paralelo (não bloqueiam a IDE)
- Preencher `docs/naming-positioning.md` → resolve D001
- Levantar stack real do operador → resolve D002
- Completar tabela copiar/reinterpretar/descartar em `docs/reference-extraction.md` → resolve D003

### Após validação visual da home no Replit
- Gate Phase 4: aprovação visual do operador
- Substituir placeholders por identidade real
- Implementar script de instalação funcional
- Deploy público

---

## Protocolo SSOT

- thread_id: 030426-164900
- master_id: 030426-164900
- ssot_version: 2.0_aprimorado
- tipo_nota: ativa
- status: conforme
- Teste idempotência: OK
