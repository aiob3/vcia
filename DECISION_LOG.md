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

**Ação paralela:** preencher `docs/naming-positioning.md` com análise de opções antes de tomar decisão.

---

## D002 — Escopo real do script de setup

**Status:** ABERTO

**Pergunta:** o que exatamente o script de instalação vai provisionar na primeira entrega funcional?

**Impacto:** Phase 4, docs técnicas, landing page de instalação.

**Opções:**
- Subset mínimo (shell + 1 AI CLI + utilitários essenciais)
- Stack completa inspirada no SetupVibe (todos os módulos)
- Stack proprietária baseada nas ferramentas já usadas pelo operador

**Ação paralela:** preencher `docs/stack-blueprint.md` — coluna Status para cada ferramenta. Quando todas saírem de `placeholder`, D002 está pronta para decisão.

---

## D003 — Reutilização da copy da referência

**Status:** ABERTO

**Pergunta:** quanto da copy do SetupVibe será reinterpretada vs substituída por narrativa própria?

**Impacto:** landing page hero, benefícios, módulos, FAQ.

**Opções:**
- Reescrever tudo do zero com posicionamento próprio
- Reinterpretar a estrutura mantendo padrões de copy que funcionam
- Usar a referência como rascunho e editar progressivamente

**Ação paralela:** completar tabela copiar/reinterpretar/descartar em `docs/reference-extraction.md`.

---

## D004 — Ambiente principal de implementação

**Status:** DECIDIDO  
**Decisão:** Replit para prototipagem inicial (Phase 3)  
**Decidido por:** operador  
**Data:** 03/04/26

**Pergunta original:** onde a fase de implementação será conduzida inicialmente?

**Racional:** velocidade de validação visual e facilidade de compartilhamento para feedback rápido. O Replit não é o destino final — é a arena de validação do prototype antes de qualquer ambiente de produção.

**Alternativas descartadas:**
- IDE local: requer config, menos ágil para validação visual
- GitHub Codespaces: overhead de configuração desnecessário na fase de prototipagem

---

## D005 — Protocolo de escalonamento dos agentes

**Status:** DECIDIDO  
**Decisão:** agente pausa, registra no DECISION_LOG e oferece 2-3 opções ao operador antes de prosseguir em decisões estruturais; continua com tasks independentes se a lacuna não bloquear tudo  
**Decidido por:** operador  
**Data:** 03/04/26

**Pergunta original:** quando um agente encontra uma lacuna ou decisão aberta, qual é o protocolo padrão?

**Ação paralela:** protocolo documentado em `AGENT_ONBOARDING.md` e `prompts/ide-agent-system.md`.

---

## Histórico de racional narrativo

> Seção preservada do setupvibe-workflow — registra o racional qualitativo das primeiras decisões antes da formalização estrutural acima.

### #ID 030426-152700 | SetupVibe como ponto de partida

**Decisão:** usar o SetupVibe como referência estrutural e de posicionamento, não como template de cópia direta.  
**Racional:** a proposta combina landing page de aquisição, documentação técnica e funil de comunidade de forma coesa. O valor para o workflow interno está na estrutura narrativa e no modelo em camadas, não nos assets visuais.  
**Alternativas descartadas:**
- Partir de template genérico de SaaS → perderia especificidade de dev tooling
- Construir do zero sem referência → aumentaria tempo de validação do racional

### #ID 030426-154300 | Onboarding como fechamento de contexto

**Decisão:** tratar onboarding não como "boas-vindas" mas como mecanismo formal de fechamento de contexto antes da execução na IDE.  
**Racional:** o processo de trabalho estabelecido (KTX, templates, prototipagem antes de MVP) exige que o contexto esteja canônico antes de delegar para agentes. Um repositório estruturado serve como SSOT para todos os agentes downstream.  
**Alternativas descartadas:**
- Ir direto para IDE sem documentar → perderia rastreabilidade
- Documentar depois da prototipagem → agentes trabalhariam sem contexto estável

### #ID 030426-164300 | Replit como ambiente de prototipagem (= D004 decidido)

**Decisão:** Replit para Phase 3, antes de qualquer ambiente de produção.  
**Tabela de bifurcação que levou à decisão:**

| Critério | Partir para IDE | Iterar mais |
|----------|----------------|-------------|
| Racional documentado | ✅ | — |
| Stack real definida | placeholders ⚠️ | seria necessário |
| Identidade visual | não definida ⚠️ | opcional p/ prototype |
| Comando de install | não testado ⚠️ | seria necessário p/ Fase 3+ |
| Blocos da home | mapeados ✅ | — |
| AGENT_ONBOARDING | completo ✅ | poderia refinar |

**Conclusão:** partir para IDE com stack em placeholder é válido — o objetivo da Phase 3 é validar estrutura visual e narrativa. Identidade e comando real vêm na Phase 4.
