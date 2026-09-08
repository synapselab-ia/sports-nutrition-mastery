# CLAIM LEDGER

Registro canônico de afirmações científicas materiais do projeto.

## Estados

- `PROVISIONAL` — claim ainda em pesquisa/QA;
- `SUPPORTED` — sustentado no escopo definido;
- `CONTESTED` — literatura relevante conflitante;
- `WEAK` — suporte limitado/indireto;
- `REJECTED` — conjunto de evidências não sustenta o claim no escopo definido;
- `RETIRED` — claim substituído/reformulado.

## Template

```text
CLAIM-ID:
Claim:
Category: MECHANISM | ASSOCIATION | CAUSAL_EFFECT | PRACTICAL_RECOMMENDATION | SAFETY | NULL_OR_NEGATIVE
Status:
Certainty: HIGH | MODERATE | LOW | VERY_LOW
Population/context:
Outcome:
Scope/conditions:
Key evidence:
Contrary evidence:
Limitations:
Dependent modules:
Last reviewed: YYYY-MM-DD
```

Nenhum claim deve ser ampliado além da população, intervenção, dose, contexto e desfecho efetivamente sustentados.
