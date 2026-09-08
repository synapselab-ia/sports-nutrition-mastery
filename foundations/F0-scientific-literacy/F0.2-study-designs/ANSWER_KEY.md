# F0.2 — Gabarito comentado

Este gabarito descreve respostas **aceitáveis** e os critérios de raciocínio esperados. Em perguntas abertas, não existe uma única redação obrigatória.

O critério principal é: **classificar pela arquitetura do estudo e preservar os limites de inferência**.

---

# Parte A — Recuperação ativa

## A1

**Intervenção** é uma condição deliberadamente aplicada/atribuída como parte do estudo. **Exposição** é uma característica, comportamento ou condição observada sem que o pesquisador necessariamente a tenha atribuído.

A mesma variável pode ser intervenção em um estudo e exposição em outro; o que importa é como o contraste foi produzido.

## A2

Randomização usa um mecanismo aleatório para determinar a alocação. Sua vantagem causal introdutória é tornar a alocação independente, em expectativa, das características prévias dos participantes, fortalecendo a comparabilidade causal dos grupos.

Não garante igualdade numérica perfeita no baseline, adesão, ausência de perdas, boa mensuração, representatividade ou execução correta.

## A3

**Between-subject:** pessoas diferentes fornecem dados das condições comparadas.

**Within-subject:** a mesma pessoa fornece dados em mais de uma condição e é comparada consigo mesma.

## A4

**Carryover** é a persistência do efeito de uma condição em um período posterior, interferindo na resposta à condição seguinte.

## A5

**Washout** é o intervalo planejado para reduzir suficientemente o efeito residual da condição anterior antes do próximo período. Sua duração depende da biologia/efeito relevante; não existe duração universal.

## A6

**Unidade de alocação** é quem/qual entidade recebe a condição designada. **Unidade de observação** é onde o outcome é medido.

Em cluster trials, por exemplo, uma academia pode ser alocada e atletas individuais observados.

## A7

A diferença é a forma de amostragem/entrada no desenho:

- cohort retrospectiva: define população/exposição em um ponto inicial passado e reconstrói outcomes posteriores;
- case-control: seleciona primeiro por status de outcome (casos/controles) e então reconstrói exposições anteriores.

“Usar dados antigos” não define case-control.

## A8

Em cross-sectional, exposição e outcome são medidos no mesmo recorte temporal ou em janela próxima, portanto frequentemente não é possível estabelecer qual veio primeiro. Isso limita temporal ordering e facilita ambiguidade de reverse causation.

## A9

Em um factorial 2 × 2, participantes são randomizados em relação a dois fatores, produzindo quatro combinações: nenhum, A, B ou A+B. O desenho permite investigar efeitos de cada fator e possíveis interações.

## A10

O target-trial framework tenta tornar explícito qual ensaio randomizado hipotético responderia à pergunta causal: elegibilidade, estratégias, início do seguimento, outcome, horizonte, contraste/estimand e análise-alvo. Depois se avalia se dados observacionais podem emular essa arquitetura.

---

# Parte B — Oito estudos, oito limites

## B1 — 12 semanas, dois grupos

**Desenho:** randomized parallel-group trial.

**Comparação:** between-subject.

**Inferência mais forte:** efeito do contraste randomizado A versus B sobre a mudança no 1RM em 12 semanas, para a população e condições estudadas, desde que condução/análise sejam adequadas.

**Inferência não estabelecida automaticamente:** que o resultado se aplica a qualquer atleta, dose, protocolo, outcome ou duração; ou que randomização elimina todos os demais problemas metodológicos.

**Pontuação completa exige:** reconhecer randomização + paralelo + limite de generalização/validade total.

## B2 — duas condições na mesma pessoa

**Desenho:** randomized crossover trial.

**Comparação:** within-subject.

**Inferência mais forte:** diferença entre A e B dentro dos mesmos ciclistas, sob sequências/períodos adequados e com carryover suficientemente controlado.

**Inferência não estabelecida automaticamente:** que crossover é sempre superior a paralelo, ou que qualquer washout garante ausência de carryover.

**Ponto adicional aceitável:** period effects precisam ser considerados conceitualmente.

## B3 — academias randomizadas

**Desenho:** cluster-randomized trial.

**Comparação:** entre clusters com indivíduos aninhados nos clusters.

**Unidade de alocação:** academia.

**Unidade de observação:** aluno.

**Inferência mais forte:** efeito da atribuição do programa no nível da academia sobre outcomes medidos nos alunos, com análise compatível com clustering.

**Inferência não estabelecida automaticamente:** que existem 300 unidades randomizadas independentes.

## B4 — dois fatores simultâneos

**Desenho:** randomized 2 × 2 factorial trial.

**Comparação:** múltiplos contrastes entre combinações/fatores; em geral between-subject neste exemplo.

**Inferência mais forte:** efeitos dos fatores A e B segundo comparações prespecificadas e possibilidade de avaliar se um fator modifica o efeito do outro.

**Inferência não estabelecida automaticamente:** que A+B é necessariamente a soma dos efeitos isolados.

**Ponto-chave:** interação precisa ser respeitada na interpretação.

## B5 — programa adotado sem randomização

**Desenho:** non-randomized intervention study, com grupos por campus.

**Comparação:** between-subject/entre grupos institucionais.

**Inferência mais forte:** diferença de outcomes entre os campi após implementação, com temporalidade da intervenção explícita.

**Inferência não estabelecida automaticamente:** que o programa causou toda diferença observada apenas porque um campus o recebeu e outro não.

**Erro a evitar:** chamar de RCT por existir uma intervenção.

## B6 — exposição primeiro, outcome depois

**Desenho:** retrospective cohort.

**Comparação:** grupos definidos por exposição/baseline.

**Inferência mais forte:** associação longitudinal entre exposição registrada em 2018 e outcome posterior até 2026, com temporal ordering.

**Inferência não estabelecida automaticamente:** causalidade somente porque exposição veio antes do outcome.

**Erro crítico:** classificar como case-control apenas porque os dados vêm de registros históricos.

## B7 — casos primeiro

**Desenho:** case-control.

**Comparação:** casos versus controles quanto a exposições anteriores.

**Inferência mais forte:** associação entre exposições anteriores e status de caso, com medida de associação apropriada ao desenho.

**Inferência não estabelecida automaticamente:** risco/incidência populacional direta ou causalidade automática.

**Ponto decisivo:** a seleção começou pelo outcome.

## B8 — fotografia do momento

**Desenho:** cross-sectional.

**Comparação:** associação contemporânea entre variáveis na mesma amostra.

**Inferência mais forte:** prevalência/associação no recorte temporal estudado.

**Inferência não estabelecida automaticamente:** que menor ingestão causou fadiga.

**Explicação esperada:** a direção temporal pode ser inversa ou ambas as variáveis podem refletir outro processo.

---

# Parte C — Escolha o desenho e justifique

## C1 — efeito agudo reversível

1. **Desenho:** randomized crossover trial.
2. **Condições a avaliar:** estabilidade do participante/condição ao longo dos períodos e reversibilidade do efeito; também são válidas respostas que mencionem repetibilidade do outcome, washout suficiente e risco de period effects.
3. **Problema se efeito persistir:** carryover; a resposta na segunda sessão refletiria parcialmente a primeira condição.

**Inferência correta:** crossover é eficiente aqui por comparação within-subject, mas só se a arquitetura biológica permitir reset suficiente entre sessões.

## C2 — intervenção de equipe

1. **Desenho:** cluster-randomized trial.
2. **Unidade de alocação:** equipe.
3. **Por que não tratar atletas como independentes:** atletas da mesma equipe compartilham intervenção/contexto e tendem a ter outcomes correlacionados; o desenho randomizou equipes, não indivíduos.

**Resposta excelente:** diferencia ainda unidade de observação (atleta) de unidade de alocação (equipe).

## C3 — adaptação irreversível no período

1. Crossover simples é inadequado porque hipertrofia/adaptação produzida por 16 semanas persiste; não é plausível apagar esse estado com washout curto e começar a segunda condição em baseline comparável.
2. **Desenho natural:** randomized parallel-group trial.
3. **Inferência a evitar:** generalização automática para mulheres, idosos, não treinados, outras modalidades ou outras intervenções/durações.

**Ponto principal:** o problema é irreversibilidade/persistência, não apenas escolher “washout maior”.

## C4 — outcome raro

1. **Desenho possível:** case-control, especialmente se casos raros já puderem ser identificados; uma cohort muito grande também pode ser informativa dependendo dos dados.
2. “RCT sempre é melhor” falha porque adequação depende da pergunta e da frequência/horizonte do outcome; um RCT pequeno/curto pode simplesmente não observar eventos raros suficientes.
3. **Limite causal:** associação entre exposição e evento ainda requer avaliação de comparabilidade, seleção, mensuração e confounding — conteúdo aprofundado em F0.3.

---

# Parte D — Problemas estruturais

## D1 — crossover mal escolhido

O problema central é que o outcome/intervenção produz **efeito duradouro**. Hipertrofia acumulada no primeiro período não retorna rapidamente ao estado inicial. Portanto, o pressuposto de que cada período pode fornecer uma comparação limpa/reversível falha.

Aumentar washout de sete para dez dias não resolve conceitualmente o problema. Seria necessário um intervalo suficientemente longo para desfazer adaptação — o que pode ser impraticável, biologicamente indesejável e ainda não restaurar condições comparáveis.

**Resposta completa:** identifica persistência/irreversibilidade + carryover estrutural + inadequação do crossover.

## D2 — cluster tratado como indivíduos independentes

A frase está errada porque **dez escolas**, não 1.000 alunos, foram randomizadas.

Reescrita aceitável:

> “Dez escolas foram randomizadas, cinco por braço, e aproximadamente 1.000 alunos foram observados dentro dessas escolas; a análise deve respeitar a estrutura de clustering.”

Não significa que o ensaio tenha “apenas n=10” em todo sentido estatístico; significa que a unidade de randomização é escola e que a informação dos alunos dentro de cada escola não pode ser tratada como se viesse de randomizações independentes.

---

# Parte E — Target trial + F0.1

Há várias respostas válidas. O critério é tornar a pergunta e o ensaio-alvo coerentes.

## E1 — Reconstrução da pergunta

Exemplo aceitável:

> Em atletas adultos que treinam regularmente, manter consumo diário de café da manhã segundo definição prévia, comparado a omitir café da manhã na maior parte dos dias, altera a mudança em um teste padronizado de desempenho ao longo de 12 meses?

Elementos:

- **população:** atletas adultos treinando regularmente;
- **estratégias:** consumir versus omitir café da manhã segundo regras explícitas;
- **outcome:** mudança em teste padronizado de desempenho;
- **tempo:** 12 meses.

Outras escolhas coerentes recebem pontuação completa.

## E2 — Target trial introdutório

Exemplo:

1. **Elegibilidade:** atletas adultos, rotina de treinamento definida, sem condição que torne uma das estratégias impraticável.
2. **Estratégias:** consumo diário de café da manhã padronizado versus omissão segundo protocolo definido.
3. **Início do seguimento:** data da alocação hipotética, com baseline medido antes da estratégia.
4. **Outcome:** mudança em teste padronizado de performance ou outro outcome explicitamente operacionalizado.
5. **Horizonte:** 12 meses.
6. **Contraste:** diferença entre estratégias na mudança média do outcome sob a política definida para adesão/interrupções.

O objetivo não é desenhar toda a estatística, mas mostrar que a análise observacional deve tentar corresponder a uma pergunta causal explícita.

## E3 — Limite

Target-trial emulation não randomiza pessoas retroativamente. Os dados observacionais continuam sujeitos a limitações de medição, comparabilidade, disponibilidade de variáveis e confounding não medido. O framework ajuda a especificar o desenho causal-alvo e evita alguns erros de arquitetura, mas não cria informação que os dados não possuem.

---

# Rubrica de correção

## 90–100

Classifica desenhos pela arquitetura, não por palavras-chave; distingue unidades, tempo e modo de alocação; identifica espontaneamente inferência máxima e inferência proibida; reconhece casos em que o desenho “mais prestigiado” não é o mais adequado à pergunta.

## 80–89

Competência suficiente para avançar. Pode haver imprecisões terminológicas menores, mas a lógica de desenho e limites permanece correta.

## 70–79

Compreensão parcial. Requer correção dirigida, especialmente se houver confusão entre cohort/case-control, crossover/paralelo, unidade de alocação ou temporal ordering.

## <70

A arquitetura ainda não está estável. Revisar F0.2 e resolver novos casos equivalentes.

---

# Falhas críticas

Mesmo com nota total alta, não considerar F0.2 aplicado se o estudante:

- converte associação observacional em causalidade sem justificativa adicional;
- trata randomização como prova de validade universal;
- chama cohort retrospectiva de case-control apenas por usar dados passados;
- ignora que cluster, e não indivíduo, foi randomizado;
- aceita crossover para efeito persistente sem reconhecer carryover/irreversibilidade;
- transforma resposta aguda mecanística em prova automática de outcome crônico;
- afirma que target-trial emulation elimina a necessidade de assumptions/dados adequados.

Esses erros atingem diretamente `K4`, `K6` e `K8` e devem ser corrigidos antes da progressão conceitual para F0.3.