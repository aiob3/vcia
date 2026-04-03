# DECISION_LOG — VCIA

Registro de decisões tomadas e pendências abertas. Toda decisão com impacto estrutural no projeto deve ser documentada aqui antes de ser implementada.

## Formato

```
ID: D###
Status: [ABERTO | DECIDIDO | DESCARTADO]
Pergunta: qual é a dúvida ou bifurcação?
Impacto: quais fases ou artefatos são afetados?
Opções: hipóteses levantadas
Decisão: o que foi escolhido (se já decidido)
Decidido por: operador / agente / consenso
Data: DD/MM/AA
Ação paralela: o que deve ser feito antes de integrar
```

---

## D001 — Naming e identidade própria

**Status:** ABERTO

**Pergunta:** qual é o nome definitivo, promessa central e semântica do projeto — separado da referência SetupVibe?

**Impacto:** README, landing page, copy, script de instalação, comunidade.

**Opções:**
- Manter VCIA como nome de repositório e criar branding a partir dele
- Usar VCIA como nome técnico interno e criar nome público diferente
- Definir nome completamente novo baseado na tese do projeto

**Ação paralela:** criar documento `docs/naming-positioning.md` com análise de opções antes de tomar decisão.

---

## D002 — Escopo real do script de setup

**Status:** ABERTO

**Pergunta:** o que exatamente o script de instalação vai provisionar na primeira entrega funcional?

**Impacto:** Phase 4, docs técnicas, landing page de instalação.

**Opções:**
- Subset mínimo (shell + 1 AI CLI + utilitários essenciais)
- Stack completa inspirada no SetupVibe (todos os módulos)
- Stack proprietária baseada nas ferramentas já usadas pelo operador

**Ação paralela:** levantar stack atual real do operador e mapear delta em relação à referência SetupVibe.

---

## D003 — Reutilização da copy da referência

**Status:** ABERTO

**Pergunta:** quanto da copy do SetupVibe será reinterpretada vs substituída por narrativa própria?

**Impacto:** landing page hero, benefícios, módulos, FAQ.

**Opções:**
- Reescrever tudo do zero com posicionamento próprio
- Reinterpretar a estrutura mantendo padrões de copy que funcionam
- Usar a referência como rascunho e editar progressivamente

**Ação paralela:** criar tabela copiar / reinterpretar / descartar para cada elemento extraído.

---

## D004 — Ambiente principal de implementação

**Status:** ABERTO

**Pergunta:** onde a fase de implementação será conduzida inicialmente?

**Impacto:** Phase 3, protocolo de agentes, integração com GitHub.

**Opções:**
- Replit (prototipagem rápida, sem config local)
- IDE local com sync para GitHub (VSCode / Cursor)
- GitHub Codespaces (ambiente cloud gerenciado)

**Ação paralela:** validar se o ambiente escolhido suporta o fluxo agêntico desejado antes de iniciar Phase 3.

---

## D005 — Protocolo de escalonamento dos agentes

**Status:** ABERTO

**Pergunta:** quando um agente encontra uma lacuna ou decisão aberta, qual é o protocolo padrão?

**Impacto:** Phase 3, AGENT_ONBOARDING.md, qualidade das entregas.

**Opções:**
- Agente pausa e registra no DECISION_LOG, aguarda operador
- Agente assume a hipótese mais conservadora e sinaliza no output
- Agente oferece 2-3 opções e solicita confirmação antes de prosseguir

**Ação paralela:** definir no AGENT_ONBOARDING.md o padrão esperado por tipo de lacuna.
