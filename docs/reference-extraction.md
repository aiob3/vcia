# reference-extraction.md
> Extração estrutural do modelo SetupVibe para uso como referência de partida
> #ID 030426-152700 | extração setupvibe

---

## Propósito deste documento

Registra o que foi extraído do SetupVibe como referência estrutural. Nada aqui é identidade do projeto VCIA. Este documento alimenta a análise da Camada 1 (referência observada) do workflow de 3 camadas.

---

## Estrutura de navegação

| Página | Objetivo | Componentes principais |
|--------|----------|------------------------|
| Home | Aquisição e conversão | Hero, faixa de benefícios, processo 3 passos, compatibilidade, módulos, agentes, FAQ, footer |
| Como Funciona | Explicação técnica por camada | Blueprint de stack, narrativa de benefícios operacionais |
| Ferramentas | Roadmap em estágios | Tabela técnica por estágio, racional estratégico |
| Instalar | Execução | Comando principal, fluxo 3 passos, FAQ pré-instalação, CTA comunidade |

---

## Blocos da home (mapeados)

1. **Hero** — headline forte, subtítulo orientado a transformação, 2 CTAs, badge de compatibilidade
2. **Faixa de benefícios** — Zsh/Starship, IA Integrada, Modern Unix, One-Click Setup
3. **Processo em 3 passos** — copiar comando → executar script → começar a produzir
4. **Compatibilidade por plataforma** — Windows WSL2, macOS, Linux Debian/Ubuntu
5. **Grade de módulos** — Zsh/Starship, AI CLI Tools, Modern Unix, Tmux, Ecossistema Dev, PM2, Portainer, Cronboard, Aliases & Atalhos
6. **Compatibilidade com agentes/frameworks** — Cursor, GitHub Copilot, Claude/Gemini, Node/Python/React
7. **FAQ curta**
8. **Bloco de comunidade/upsell**
9. **Footer institucional**

---

## Stack técnica anunciada

### Shell & UX Terminal
- Zsh + Oh My Zsh + Starship (preset Gruvbox)
- Plugins: zsh-autosuggestions, zsh-syntax-highlighting

### AI CLI
- Claude Code, Gemini CLI, GitHub Copilot CLI

### Runtimes
- Python 3.12 (uv), Node 24, Bun, Go, Rust, Ruby 3.3 (rbenv), PHP 8.4 + Composer

### DevOps
- Docker CE + Compose v2 + Buildx, Portainer CE, PM2, Ansible, GitHub CLI

### Produtividade CLI (Modern Unix)
- eza, bat, ripgrep, fd, zoxide, fzf, glow, LazyGit, LazyDocker, Neovim

### Infra complementar
- Tailscale, Cronboard/Crontab, htop/btop/glances/ctop
- nmap, mtr, rustscan, speedtest-cli, gping

---

## Padrões de copy que funcionam

- Linguagem de transformação, não de feature pura: vende rapidez, clareza, estado de flow
- Repetição estratégica de CTA e promessas-chave ao longo do scroll
- Páginas satélite para aprofundar sem poluir a home
- Prova social antecipada (+1000 devs, open source, seguro) para reduzir objeção

---

## Tabela copiar / reinterpretar / descartar

> Ação paralela para D003 — decidir quanto da copy será reutilizada vs substituída

| Elemento | Ação | Observação |
|----------|------|------------|
| Estrutura de 4 páginas | REINTERPRETAR | Manter lógica de funil, trocar conteúdo |
| Processo em 3 passos | REINTERPRETAR | Simplifica onboarding, adaptar verbos |
| Grade de módulos | REINTERPRETAR | Refletir stack real do operador |
| Promessa "5 minutos" | DESCARTAR | Só usar se for verdadeira no contexto |
| Métricas de comunidade (+1000 devs) | DESCARTAR | Só usar com dados reais |
| Compatibilidade WSL2/macOS/Linux | COPIAR | Tecnicamente válida se script suportar |
| Integração Claude/Gemini/Copilot | REINTERPRETAR | Refletir AI CLI realmente instalados |

---

## Lacunas identificadas

- O comando de instalação é simples na interface, mas o valor real está no script e nos dotfiles/plugins — o foco deve ser o pipeline de provisionamento, não só o front-end
- Claims comerciais e métricas de comunidade devem ser replicados apenas se verdadeiros
- A home comunica bem a promessa, mas parte da prova técnica depende de páginas satélite
