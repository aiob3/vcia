# PROJECT_SCOPE — VCIA

## Objetivo

Criar um workflow base reutilizável para inicialização de projetos de desenvolvimento com IA, que possa ser instanciado para qualquer novo projeto sem depender de contexto oral ou memória implícita do operador.

## Escopo inicial

- Definição da arquitetura de documentação (este repositório)
- Estrutura de fases e gates do projeto
- Protocolo de onboarding para agentes na IDE
- Blueprint de superfícies baseado na referência SetupVibe
- Template canônico de README, escopo, workflow e decisões
- Script de setup placeholder para validação do fluxo de instalação
- Primeira landing page funcional mínima no Replit

## O que está fora do escopo nesta fase

- Branding final e identidade visual definitiva
- Stack técnica completa e script de instalação em produção
- Integração com sistemas externos (CRM, automação, pagamentos)
- Criação de comunidade ou camada comercial
- SEO, analytics e performance de produção

## Critérios de aceitação para Phase 1

- [ ] Os 5 arquivos canônicos estão versionados no repositório
- [ ] Um agente externo consegue entender o projeto lendo apenas os arquivos-base
- [ ] As pendências de decisão estão registradas em `DECISION_LOG.md`
- [ ] O repositório pode ser clonado e usado como template para outro projeto

## Critérios de aceitação para entrega funcional (Phase 4)

- [ ] Existe uma landing page funcional com hero, módulos, instalação e FAQ
- [ ] Existe um comando de instalação documentado (ainda que placeholder)
- [ ] Existe uma página de documentação técnica da stack
- [ ] O fluxo completo é navegável sem dependência de contexto externo

## Decisões abertas (ver DECISION_LOG.md)

- D001 — Naming e identidade própria do projeto
- D002 — Escopo real do script de setup (o que será provisionado)
- D003 — Quanto da copy do SetupVibe será reinterpretada vs substituída
- D004 — Ambiente principal de implementação (Replit / IDE local / GitHub Codespaces)
