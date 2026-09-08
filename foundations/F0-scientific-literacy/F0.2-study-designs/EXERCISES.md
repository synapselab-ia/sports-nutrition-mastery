# F0.2 — Exercícios de recuperação ativa e aplicação

**Use depois de estudar `LESSON.md`.**

Não consulte `ANSWER_KEY.md` na primeira tentativa. O objetivo é classificar desenhos novos e justificar limites de inferência, não reconhecer palavras.

## Estrutura e pontuação

- Parte A — recuperação ativa: 20 pontos
- Parte B — classificar oito desenhos e limitar inferências: 40 pontos
- Parte C — escolha de desenho e arquitetura: 20 pontos
- Parte D — problemas estruturais: 10 pontos
- Parte E — target trial e integração com F0.1: 10 pontos

**Total:** 100 pontos.

### Gate local de competência

- `>= 80/100`: desempenho suficiente para seguir, desde que nenhuma falha crítica ocorra;
- `70–79`: corrigir as partes frágeis e refazer itens equivalentes;
- `< 70`: revisar F0.2 e repetir avaliação equivalente.

### Falha crítica, independentemente da nota

- concluir causalidade apenas porque uma associação observacional existe;
- tratar randomização como garantia de validade total/generalização universal;
- não distinguir cohort retrospectiva de case-control pela forma de amostragem;
- ignorar unidade de alocação em cluster-randomized trial;
- aceitar crossover para efeito irreversível/persistente sem reconhecer carryover;
- converter outcome mecanístico agudo em prova automática de adaptação crônica;
- tratar target-trial emulation como se produzisse randomização real.

Esta avaliação pode sustentar `RECALLED`/`APPLIED` quando efetivamente realizada e corrigida. Produção do material não altera o estado de aprendizagem.

---

# Parte A — Recuperação ativa — 20 pontos

Cada questão vale 2 pontos.

1. Diferencie intervenção de exposição.
2. O que significa randomização e qual é sua vantagem causal introdutória?
3. Diferencie comparação between-subject de within-subject.
4. O que é carryover em um crossover trial?
5. Qual é a função conceitual de um washout?
6. Diferencie unidade de alocação de unidade de observação.
7. Qual é a diferença estrutural entre cohort retrospectiva e case-control?
8. Qual é o principal limite temporal de um cross-sectional para inferência causal?
9. O que é um factorial 2 × 2 em linguagem simples?
10. O que o target-trial framework tenta tornar explícito antes de analisar dados observacionais?

---

# Parte B — Oito estudos, oito limites — 40 pontos

Para **cada** estudo:

1. classifique o desenho;
2. indique se a comparação principal é between-subject, within-subject ou em clusters/estrutura equivalente;
3. escreva a **inferência mais forte defensável**;
4. escreva **uma inferência tentadora que o desenho não estabelece automaticamente**.

Cada item vale 5 pontos.

## B1 — 12 semanas, dois grupos

Duzentos adultos treinados são randomizados individualmente para estratégia nutricional A ou B. Cada participante permanece na condição atribuída por 12 semanas. O outcome principal é mudança no 1RM.

## B2 — duas condições na mesma pessoa

Trinta ciclistas realizam dois contrarrelógios padronizados. Metade recebe a sequência bebida A → washout → bebida B; a outra metade recebe B → washout → A. A ordem é randomizada.

## B3 — academias randomizadas

Vinte academias são randomizadas para implementar programa educacional A ou rotina usual por seis meses. São medidos 15 alunos por academia.

## B4 — dois fatores simultâneos

Participantes são randomizados em um desenho 2 × 2 para:

- suplemento A ou placebo de A;
- estratégia B ou controle de B.

Assim existem quatro combinações possíveis.

## B5 — programa adotado sem randomização

Uma universidade implementa um programa alimentar em um campus, enquanto outro campus mantém sua rotina. A decisão não foi randomizada. Outcomes são comparados após um semestre.

## B6 — exposição primeiro, outcome depois

Um banco de dados identifica, em 2018, pessoas com alta ou baixa ingestão habitual de determinada categoria alimentar. Registros até 2026 são usados para verificar ocorrência posterior de um outcome.

## B7 — casos primeiro

Pesquisadores selecionam 400 pessoas com uma lesão rara e 800 controles provenientes da população que originou os casos. Depois comparam exposições nutricionais registradas antes da lesão.

## B8 — fotografia do momento

Em uma amostra de atletas, ingestão energética atual e presença atual de fadiga são medidas na mesma semana. Os autores encontram associação entre menor ingestão e maior fadiga.

---

# Parte C — Escolha o desenho e justifique — 20 pontos

Cada questão vale 5 pontos.

## C1 — efeito agudo reversível

Você quer estimar se duas bebidas diferentes alteram o desempenho em um teste de ciclismo realizado duas horas após ingestão. O efeito esperado é transitório e cada participante pode repetir o teste em condições padronizadas.

1. Qual desenho randomizado pode ser especialmente eficiente?
2. Quais duas condições precisam ser avaliadas antes de escolhê-lo?
3. Qual problema surgiria se o efeito da primeira bebida persistisse na segunda sessão?

## C2 — intervenção de equipe

Um protocolo nutricional será implementado por treinadores em equipes inteiras. Individualizar a intervenção dentro da mesma equipe provavelmente causaria forte contaminação entre atletas.

1. Qual desenho randomizado é natural?
2. Qual é a unidade de alocação?
3. Por que não se pode analisar todos os atletas como unidades randomizadas independentes?

## C3 — adaptação irreversível no período

Você quer comparar dois programas de 16 semanas para hipertrofia. O ganho estrutural de uma fase não desapareceria rapidamente antes de uma segunda condição.

1. Por que um crossover simples é inadequado?
2. Qual desenho randomizado é mais natural?
3. Qual inferência tentadora deve ser evitada se a amostra incluir apenas homens jovens treinados?

## C4 — outcome raro

Um evento adverso é muito raro e pode aparecer anos depois de uma exposição. Um RCT típico seria curto e pequeno para observar número suficiente de eventos.

1. Que desenho observacional pode ser eficiente se casos já puderem ser identificados?
2. Por que isso mostra que “RCT sempre é o melhor desenho” é uma regra inadequada?
3. Qual inferência causal ainda exige cuidado adicional?

---

# Parte D — Problemas estruturais — 10 pontos

Cada questão vale 5 pontos.

## D1 — crossover mal escolhido

Um estudo avalia um programa de treinamento de oito semanas em crossover. Os participantes fazem programa A por oito semanas, têm sete dias de washout e depois programa B por oito semanas. O outcome é hipertrofia.

Explique por que o problema não é simplesmente “washout curto”. Qual pressuposto estrutural do crossover provavelmente falha?

## D2 — cluster tratado como indivíduos independentes

Dez escolas são randomizadas, cinco por braço. Cada escola fornece 100 alunos. Um resumo diz:

> “O ensaio randomizou 1.000 participantes independentes.”

Explique por que a frase é estruturalmente incorreta e como você a reescreveria.

---

# Parte E — Target trial + F0.1 — 10 pontos

Considere a pergunta vaga:

> “Pular o café da manhã causa pior desempenho esportivo no longo prazo?”

Não há RCT longo disponível; existe uma grande base observacional com hábitos alimentares e resultados de performance ao longo de anos.

## E1 — Reconstrução da pergunta — 4 pontos

Transforme a alegação em uma pergunta mais precisa, definindo pelo menos:

- população;
- estratégias comparadas;
- outcome;
- horizonte temporal.

## E2 — Target trial introdutório — 4 pontos

Especifique, em linguagem simples, o ensaio-alvo hipotético:

1. elegibilidade;
2. estratégias;
3. início do seguimento;
4. outcome;
5. horizonte;
6. contraste de interesse.

## E3 — Limite — 2 pontos

Explique por que usar o target-trial framework **não** transforma os dados observacionais em um RCT real.

---

# Autoauditoria antes do gabarito

Antes de abrir `ANSWER_KEY.md`, confira se você:

- identificou **como o contraste foi criado**;
- separou randomizado de não randomizado;
- diferenciou cohort retrospectiva de case-control pela amostragem;
- distinguiu between-subject de within-subject;
- identificou unidade de alocação em clusters;
- verificou temporal ordering;
- questionou washout/carryover em crossover;
- não converteu estudo agudo em conclusão crônica;
- não usou “RCT” como sinônimo de “verdade”;
- escreveu para cada desenho uma inferência permitida e uma inferência proibida.