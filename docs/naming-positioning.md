# naming-positioning.md
> Análise de naming e posicionamento para D001
> Atividade paralela obrigatória antes de avançar para Phase 3

---

## Status

Atividade paralela ativa. Resultado desta análise resolve **D001** no DECISION_LOG.

---

## O que precisamos definir

1. Nome definitivo (público)
2. Promessa central (1 frase)
3. Para quem é (público-alvo primário)
4. O que diferencia do SetupVibe e similares

---

## Opções de naming

| Opção | Semântica | Prós | Contras |
|-------|-----------|------|---------|
| **VCIA** (manter) | Sigla interna, técnica | Já versionado no GitHub, neutro | Sem significado imediato para usuário |
| Nome novo | Identidade própria | Diferenciação clara | Requer rename do repo |
| VCIA como técnico + nome público | Separação interna/externo | Flexível | Aumenta complexidade de comunicação |

---

## Campo para preencher (operador)

```yaml
nome_publico: ""
promessa_central: ""
publico_primario: ""
diferenciacao: ""
aprovado_em: ""
```

---

## Testes de mensagem (rascunho)

> Testar se o projeto consegue ser explicado sem citar SetupVibe como referência:

- "[Nome] é um ambiente de desenvolvimento com IA pronto em X minutos, pensado para [público]."
- "Diferente de outras soluções, [Nome] [diferencial único]."

**Gate D001:** o nome e a promessa passam no teste acima sem precisar de contexto adicional.
