# phase-01-landing.md
> Prompt específico para o agente da Phase 1 — Landing base no Replit

---

## Contexto da fase

**phase_id:** p4 (Phase 4 — Implementação controlada, landing base)
**Ambiente:** Replit
**Repositório:** https://github.com/aiob3/vcia

---

## Objective

Criar a estrutura HTML/CSS/JS base da landing page inspirada no SetupVibe, com identidade de placeholder para VCIA, pronta para personalização progressiva.

---

## Inputs

- `docs/reference-extraction.md` — blocos mapeados e padrões de copy
- `docs/product-blueprint.md` — épico 1 (Landing base) e fluxo do usuário
- Decisões: D001 pendente (usar placeholder `[NOME]`), D002 pendente (usar stack placeholder)

---

## Tasks

- [ ] Criar `src/landing/index.html` com estrutura semântica
- [ ] Implementar header com navegação (Home, Como Funciona, Ferramentas, Instalar)
- [ ] Implementar hero: headline placeholder, subtítulo, 2 CTAs, badge de compatibilidade
- [ ] Implementar faixa de 4 benefícios
- [ ] Implementar processo em 3 passos
- [ ] Implementar grade de módulos (8-10 cards placeholder)
- [ ] Implementar bloco de compatibilidade com agentes/IDEs
- [ ] Implementar FAQ básica (3-5 perguntas)
- [ ] Implementar footer com links
- [ ] Toggle dark/light mode funcional
- [ ] Responsivo mobile-first

---

## Outputs esperados

- `src/landing/index.html`
- `src/landing/style.css`
- `src/landing/main.js`

---

## Open questions (não bloquear, sinalizar)

- D001: nome definitivo → usar `[NOME]` como placeholder
- D002: stack real → usar lista do reference-extraction.md como placeholder
- D003: copy própria → usar estrutura do SetupVibe como rascunho, marcar com `<!-- TODO: reescrever -->`

---

## Definition of done

- [ ] Todos os 9 blocos da home estão presentes
- [ ] Toggle dark/light funciona
- [ ] Layout responsivo funciona em 375px e 1280px
- [ ] Nenhuma imagem quebrada ou link morto
- [ ] Placeholders claramente marcados com `[NOME]` ou `<!-- TODO -->`
- [ ] Commit com `[p4] feat: landing page base inicial`
