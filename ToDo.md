gora eu não iria diretamente para a Fundamentação Teórica. Antes, eu fecharia algumas decisões que vão determinar boa parte do restante do TCC.

Eu seguiria esta ordem:

1. Definir os datasets

Esse é o próximo passo mais importante.

Você já decidiu que quer:

IEEE-CIS Fraud Detection;
uma segunda base com atributos mais interpretáveis;
comparar abordagens supervisionadas e não supervisionadas.

Agora precisamos definir a segunda base e verificar, para ambas:

quantidade de registros;
quantidade de fraudes;
proporção entre classes;
quantidade e significado dos atributos;
valores ausentes;
atributos categóricos/numéricos;
existência de identificadores;
possibilidade de vazamento de dados (data leakage);
se a base é adequada para os algoritmos que você pretende testar.

Eu faria uma tabela de caracterização das bases no TCC posteriormente.

2. Fazer uma pesquisa bibliográfica direcionada

Depois dos datasets, eu faria a pesquisa dos trabalhos relacionados.

Mas não simplesmente "ler artigos sobre fraude". A pesquisa deveria responder:

Quais algoritmos estão sendo utilizados para detecção de fraude e como eles estão sendo avaliados?

Para cada trabalho, registre pelo menos:

Informação	Exemplo
Autor/ano	Silva et al. (2024)
Dataset	Credit Card Fraud
Tipo	Supervisionado
Algoritmo	Random Forest
Pré-processamento	SMOTE
Métricas	Precision, Recall, F1
Resultado	...
Observações	...

Isso vai te ajudar diretamente a escolher os algoritmos.

3. Definir os algoritmos

Só depois da pesquisa bibliográfica eu fecharia os algoritmos.

Como você quer pelo menos 1–2 supervisionados e 1–2 não supervisionados, poderíamos chegar, por exemplo, a algo conceitualmente assim:

Supervisionados

Logistic Regression
Random Forest
XGBoost

Não supervisionados

Isolation Forest
One-Class SVM
K-Means

Não estou dizendo que esses serão os escolhidos. A ideia é deixar a literatura e as características dos datasets guiarem a seleção.

Um ponto importante: algoritmos não supervisionados podem exigir uma discussão diferente, porque "fraude" normalmente é uma classe conhecida nos datasets. Precisamos definir cuidadosamente como vamos utilizar os rótulos apenas para avaliação, sem fornecê-los ao algoritmo durante o treinamento.

4. Definir exatamente a pergunta de pesquisa

Depois disso, eu formalizaria o problema central do TCC.

Algo próximo de:

Como diferentes algoritmos de aprendizado de máquina supervisionado e não supervisionado se comportam na detecção de transações fraudulentas em bases de dados com características distintas?

Podemos refiná-la depois.

Isso é importante porque cada parte do TCC precisa responder a essa pergunta.

5. Estruturar a Fundamentação Teórica

Só então eu começaria a escrever o capítulo 2.

Eu sugiro inicialmente:

2 FUNDAMENTAÇÃO TEÓRICA

2.1 Transações financeiras e pagamentos digitais
2.2 Fraudes em transações financeiras
2.3 Detecção de fraudes
    2.3.1 Prevenção e detecção
    2.3.2 Falsos positivos e falsos negativos
    2.3.3 Desbalanceamento de classes
    2.3.4 Mudança de padrões
2.4 Aprendizado de máquina
    2.4.1 Aprendizado supervisionado
    2.4.2 Aprendizado não supervisionado
2.5 Algoritmos de classificação
    2.5.1 [Algoritmo]
    2.5.2 [Algoritmo]
2.6 Detecção de anomalias
    2.6.1 [Algoritmo]
    2.6.2 [Algoritmo]
2.7 Métricas de avaliação
    2.7.1 Matriz de confusão
    2.7.2 Precision
    2.7.3 Recall
    2.7.4 F1-score
    2.7.5 ROC-AUC
    2.7.6 PR-AUC

Os algoritmos só entram depois de decidirmos quais serão.

6. Depois: Trabalhos Relacionados

Aqui entraria aquela ideia que você teve de analisar a frequência de utilização dos algoritmos.

Podemos fazer algo bem interessante:

Pesquisa bibliográfica → tabela dos trabalhos → frequência dos algoritmos → justificativa da seleção dos seus algoritmos.

Por exemplo:

Artigos encontrados
        ↓
Seleção dos trabalhos relevantes
        ↓
Extração das informações
        ↓
Algoritmos utilizados
        ↓
Frequência de utilização
        ↓
Características dos algoritmos
        ↓
Seleção dos modelos do TCC

Isso cria uma conexão muito boa entre o capítulo 3 e o capítulo experimental.