# PROJECT SPEC — Sports Nutrition Mastery

## 1. Missão

Construir uma base pública, longitudinal, versionada e baseada em evidências para domínio avançado de ciência da nutrição esportiva.

O sistema deve funcionar simultaneamente como:

- currículo estruturado;
- biblioteca curada de fontes;
- sistema de produção de aulas autossuficientes;
- sistema de análise crítica de evidência;
- mapa de claims e grau de certeza;
- ambiente de avaliação e domínio;
- memória persistente entre chats;
- gerador de pacotes de estudo para NotebookLM.

## 2. Meta de aprendizagem

O estudante deve progredir até conseguir:

1. explicar fundamentos bioquímicos e fisiológicos relevantes;
2. explicar mecanismos sem depender de slogans;
3. interpretar desenho de estudo, estatística e limitações;
4. diferenciar plausibilidade mecanística de evidência de desfecho;
5. comparar consensos, revisões, meta-análises e estudos primários;
6. estimar força e aplicabilidade de uma conclusão;
7. reconhecer pseudociência e extrapolação indevida;
8. aplicar conhecimento a casos educacionais complexos;
9. atualizar conclusões quando a literatura muda.

## 3. Não é um curso de resumos

Cada módulo deve ensinar o conteúdo necessário para compreensão real. Pré-requisitos estruturais não podem ser apenas citados; devem ser ensinados antes ou dentro da progressão curricular.

Progressão pedagógica padrão:

`linguagem acessível → conceito → mecanismo → linguagem técnica → evidência → crítica → aplicação → integração`

## 4. Verdade científica e incerteza

O sistema deve separar explicitamente:

- fato/fundamento consolidado;
- recomendação de consenso;
- inferência mecanística;
- resultado experimental;
- associação observacional;
- evidência emergente;
- controvérsia;
- hipótese não demonstrada.

Nunca converter ausência de evidência em evidência de ausência, nem associação em causalidade, nem significância estatística em relevância prática.

## 5. Claims rastreáveis

Afirmações materiais devem poder ser registradas em `evidence/CLAIM_LEDGER.md` com:

- identificador;
- claim;
- população/contexto;
- desfecho;
- tipo de evidência;
- grau de certeza;
- principais fontes;
- limitações;
- data da última revisão.

## 6. Arquitetura curricular

O conhecimento é organizado por dependência conceitual, não por semestre.

Áreas principais:

- `foundations/` — método científico, bioquímica, fisiologia e metabolismo;
- `domains/` — energia, macronutrientes, micronutrientes, hidratação, suplementos e outros domínios;
- `applications/` — hipertrofia, força, endurance, composição corporal, esportes específicos e cenários ambientais;
- `controversies/` — temas com debate científico relevante;
- `evidence/` — claims, fontes e mapas de evidência;
- `study/` — domínio, erros, histórico e pacotes NotebookLM.

## 7. Produção versus aprendizagem

A produção curricular e a validação de aprendizagem são trilhas separadas.

Uma aula pode ser produzida sem que a anterior esteja testada. Porém, `MASTERED` exige evidência real de desempenho.

## 8. NotebookLM

NotebookLM é uma camada de estudo, não a fonte canônica.

O repositório define:

- quais fontes entram;
- qual objetivo de aprendizagem;
- quais perguntas devem ser exploradas;
- quais limitações devem ser observadas.

Cada pacote deve ter manifesto rastreável no repositório.

## 9. Repositório público

Nenhum dado pessoal, clínico ou sensível deve ser persistido. O projeto registra apenas estado acadêmico não sensível e artefatos científicos públicos/licenciados de forma compatível.

## 10. Limites profissionais

O projeto busca domínio científico e educacional. Ele não confere habilitação profissional, não substitui prática supervisionada e não deve ser usado para representar exercício profissional regulamentado que exija credencial específica.
