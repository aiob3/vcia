# product-blueprint.md
> Mapa de superfícies, componentes e fluxo do produto VCIA
> Pendente de aprovação do gate Phase 2

---

## Status

Este documento é o entregável principal da **Phase 2**. As seções marcadas como `[RASCUNHO]` precisam ser preenchidas após aprovação das decisões D001 (naming) e D002 (escopo do script) no DECISION_LOG.

---

## Superfícies do produto

| ID | Superfície | Objetivo | Status |
|----|-----------|----------|--------|
| S1 | Landing home | Aquisição e conversão | [RASCUNHO] |
| S2 | Como funciona | Explicação técnica das camadas | [RASCUNHO] |
| S3 | Ferramentas | Blueprint da stack por estágio | [RASCUNHO] |
| S4 | Instalar | Execução do setup | [RASCUNHO] |

---

## Componentes globais

- Header com navegação principal
- Toggle dark/light mode
- CTA persistente / sticky
- Bloco de comunidade reutilizável
- Footer com links sociais e institucionais

---

## Fluxo principal do usuário

```
Descoberta → Home (S1)
    ↓
Entendimento → Como funciona (S2)
    ↓
Confiança → Ferramentas (S3)
    ↓
Ação → Instalar (S4)
    ↓
Expansão → Comunidade / Mentoria
```

---

## Backlog inicial por épico

### Épico 1: Landing base
- [ ] Hero com headline, subtítulo, 2 CTAs
- [ ] Faixa de benefícios (4 itens)
- [ ] Processo em 3 passos
- [ ] Compatibilidade por plataforma
- [ ] Grade de módulos
- [ ] Compatibilidade com agentes/IDEs
- [ ] FAQ
- [ ] Footer

### Épico 2: Página de instalação
- [ ] Comando único de instalação (placeholder)
- [ ] Fluxo em 3 passos com detalhes
- [ ] Matriz de compatibilidade
- [ ] FAQ pré-instalação
- [ ] CTA para comunidade/suporte

### Épico 3: Blueprint técnico
- [ ] Narrativa de camadas do setup
- [ ] Tabela de stack por estágio
- [ ] Racional de escolhas técnicas

### Épico 4: Identidade e branding
- [ ] Naming definitivo (depende de D001)
- [ ] Copy com promessa própria
- [ ] Visual diferenciado do SetupVibe

---

## Matriz de dependências

| Entregável | Depende de | Bloqueia |
|-----------|-----------|----------|
| Comando de install | D002 (stack real) | S4 completo |
| Copy hero | D001 (naming) + D003 (copy) | S1, S2, S3 |
| Grade de módulos | D002 (stack) | S1, S3 |
| Protocolo de agentes IDE | D005 (escalonamento) | Phase 3 abertura |
