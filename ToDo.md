# Planejamento Inicial e Decisões Estratégicas para o TCC

Antes de prosseguir diretamente para a elaboração da Fundamentação Teórica, é necessário alinhar decisões estratégicas que orientarão todo o desenvolvimento metodológico e experimental do trabalho.

---

## 1. Definir os Datasets

Este é o próximo passo fundamental.

### Decisões prévias:
* Utilização da base **IEEE-CIS Fraud Detection**;
* Definição de uma **segunda base de dados** com atributos mais interpretáveis;
* Comparação entre abordagens **supervisionadas** e **não supervisionadas**.

### Aspectos a verificar em ambas as bases:
* Quantidade total de registros;
* Quantidade e proporção entre as classes (casos de fraude vs. não-fraude);
* Quantidade e significado dos atributos (numéricos e categóricos);
* Presença de valores ausentes (*missing values*);
* Existência de identificadores/chaves primárias;
* Possibilidade de vazamento de dados (*data leakage*);
* Adequação da base aos algoritmos que serão testados.

> **Nota:** Posteriormente, será estruturada uma tabela comparativa de caracterização dos *datasets*.

---

## 2. Pesquisa Bibliográfica Direcionada

Levantamento dos trabalhos relacionados com o objetivo central de responder:

> **Quais algoritmos estão sendo utilizados para detecção de fraude e como eles estão sendo avaliados?**

### Estrutura para registro de cada artigo lido:

| Informação | Exemplo |
| :--- | :--- |
| **Autor / Ano** | Silva et al. (2024) |
| **Dataset** | Credit Card Fraud |
| **Tipo** | Supervisionado |
| **Algoritmo** | Random Forest |
| **Pré-processamento** | SMOTE |
| **Métricas** | Precision, Recall, F1 |
| **Resultado** | ... |
| **Observações** | ... |

---

## 3. Definir os Algoritmos

A seleção final dos algoritmos será respaldada pela revisão bibliográfica e pelas características das bases de dados. 

### Exemplos de abordagens sob análise:

* **Supervisionados:**
  * Logistic Regression
  * Random Forest
  * XGBoost

* **Não Supervisionados:**
  * Isolation Forest
  * One-Class SVM
  * K-Means

> **Atenção:** Algoritmos não supervisionados exigirão uma consideração especial na metodologia: a variável alvo (rótulo de fraude) será utilizada exclusivamente na etapa de **avaliação**, sem ser fornecida durante o treinamento do modelo.

---

## 4. Definir Exatamente a Pergunta de Pesquisa

Formalização do problema central a ser respondido ao longo do trabalho:

> *"Como diferentes algoritmos de aprendizado de máquina supervisionado e não supervisionado se comportam na detecção de transações fraudulentas em bases de dados com características distintas?"*

---

## 5. Estruturar a Fundamentação Teórica

Proposta de estrutura preliminar para o Capítulo 2:

```
2 FUNDAMENTAÇÃO TEÓRICA
│
├── 2.1 Transações financeiras e pagamentos digitais
├── 2.2 Fraudes em transações financeiras
├── 2.3 Detecção de fraudes
│   ├── 2.3.1 Prevenção e detecção
│   ├── 2.3.2 Falsos positivos e falsos negativos
│   ├── 2.3.3 Desbalanceamento de classes
│   └── 2.3.4 Mudança de padrões
├── 2.4 Aprendizado de máquina
│   ├── 2.4.1 Aprendizado supervisionado
│   └── 2.4.2 Aprendizado não supervisionado
├── 2.5 Algoritmos de classificação
│   ├── 2.5.1 [Algoritmo Definido A]
│   └── 2.5.2 [Algoritmo Definido B]
├── 2.6 Detecção de anomalias
│   ├── 2.6.1 [Algoritmo Definido C]
│   └── 2.6.2 [Algoritmo Definido D]
└── 2.7 Métricas de avaliação
    ├── 2.7.1 Matriz de confusão
    ├── 2.7.2 Precision
    ├── 2.7.3 Recall
    ├── 2.7.4 F1-score
    ├── 2.7.5 ROC-AUC
    └── 2.7.6 PR-AUC
```

---

## 6. Trabalhos Relacionados e Justificativa dos Modelos

Conexão entre a revisão da literatura e o desenho experimental através da análise da frequência de uso dos algoritmos.

```
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
```
