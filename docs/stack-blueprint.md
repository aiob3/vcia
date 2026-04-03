# stack-blueprint.md

> Stack técnica de referência organizada por módulo/estágio  
> **Origem:** migrado de `aiob3/setupvibe-workflow` — arquivo único não coberto pelo reference-extraction  
> Baseada no SetupVibe — substituir pelos valores reais do workflow interno antes da Phase 4  
> Relacionado: `docs/reference-extraction.md` (contexto narrativo), D002 (escopo real do script)

## ⚠️ Status: PLACEHOLDER — revisar e preencher antes de iniciar Phase 4

Este arquivo contém a stack de referência extraída do SetupVibe.  
Antes de abrir o Replit para fase de personalização, substitua cada item pelo equivalente real do seu workflow.  
Use a coluna **Status** para rastrear: `placeholder` → `confirmado` → `substituído` → `removido`

---

## Estágio 1 — Shell & UX de terminal

| Ferramenta | Papel | Status |
|------------|-------|--------|
| Zsh | Shell principal | placeholder |
| Oh My Zsh | Framework de plugins | placeholder |
| Starship | Prompt customizado (preset Gruvbox) | placeholder |
| zsh-autosuggestions | Sugestão de comandos | placeholder |
| zsh-syntax-highlighting | Highlight em tempo real | placeholder |

## Estágio 2 — AI CLI Tools

| Ferramenta | Papel | Status |
|------------|-------|--------|
| Claude Code | Agente de código via CLI | placeholder |
| Gemini CLI | Agente Google via terminal | placeholder |
| GitHub Copilot CLI | Sugestões inline no terminal | placeholder |

## Estágio 3 — Linguagens & Runtimes

| Runtime | Versão referência | Status |
|---------|------------------|--------|
| Python | 3.12 via uv | placeholder |
| Node.js | 24 | placeholder |
| Bun | latest | placeholder |
| Go | latest | placeholder |
| Rust | latest | placeholder |
| Ruby | 3.3.0 via rbenv | placeholder |
| PHP | 8.4 + Composer | placeholder |

## Estágio 4 — DevOps

| Ferramenta | Papel | Status |
|------------|-------|--------|
| Docker CE | Containers | placeholder |
| Docker Compose v2 | Orquestração local | placeholder |
| Portainer CE | UI de containers | placeholder |
| PM2 | Process manager Node | placeholder |
| Ansible | Automação de infra | placeholder |
| GitHub CLI | Operações Git/GitHub | placeholder |

## Estágio 5 — Produtividade CLI

| Ferramenta | Papel | Status |
|------------|-------|--------|
| eza | ls moderno | placeholder |
| bat | cat com syntax highlight | placeholder |
| ripgrep | grep em Rust | placeholder |
| fd | find moderno | placeholder |
| zoxide | cd inteligente | placeholder |
| fzf | fuzzy finder | placeholder |
| glow | Markdown no terminal | placeholder |
| LazyGit | Git TUI | placeholder |
| LazyDocker | Docker TUI | placeholder |
| Neovim | Editor modal | placeholder |

## Estágio 6 — Infra complementar

| Ferramenta | Papel | Status |
|------------|-------|--------|
| Cronboard/Crontab | Agendamento | placeholder |
| Tailscale | VPN mesh | placeholder |
| OpenSSH | Acesso remoto | placeholder |
| htop/btop/glances | Monitoramento de recursos | placeholder |
| nmap/rustscan | Network scanning | placeholder |
| speedtest-cli/gping | Diagnóstico de rede | placeholder |

---

## Como usar este arquivo

1. Para cada item com `placeholder`, confirme se a ferramenta fará parte do seu script real
2. Mude o status para `confirmado` (vai entrar), `substituído` (troca por outro) ou `removido` (fora do escopo)
3. Quando todas as linhas saírem de `placeholder`, este arquivo alimenta D002 (escopo do script) e desbloqueia Phase 4
