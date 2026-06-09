# NaiveBayes

Este README documenta apenas o notebook `NaiveBayes.ipynb`, que implementa um classificador Naive Bayes com o conjunto de dados `Credit.csv`.

## Objetivo

Treinar e avaliar um modelo `GaussianNB` para prever a classe de crédito a partir de atributos do conjunto de dados.

## Requisitos

- Python 3.x
- pandas
- scikit-learn

## Uso

1. Abra o notebook `NaiveBayes.ipynb` em Jupyter ou no VS Code.
2. Verifique o caminho do arquivo `Credit.csv` e ajuste se necessário.
3. Execute as células na ordem para carregar dados, pré-processar, treinar e avaliar o modelo.

## O que o notebook faz

1. Importa `pandas`, `LabelEncoder`, `train_test_split`, `GaussianNB`, `confusion_matrix` e `accuracy_score`.
2. Lê os dados de `Credit.csv`.
3. Separa os atributos (`previsores`) e a classe alvo (`classe`).
4. Converte atributos categóricos em valores numéricos usando `LabelEncoder`.
5. Divide os dados em treino e teste com `train_test_split`.
6. Treina o modelo `GaussianNB`.
7. Faz previsões no conjunto de teste.
8. Avalia o resultado usando matriz de confusão e taxa de acerto.

## Observação importante

Se ocorrer erro ao atribuir os valores codificados em colunas com `dtype=string`, converta a coluna ou o DataFrame para `object` antes de usar `LabelEncoder`:

```python
previsores = previsores.astype(object)
```

## Licença

Projeto para estudo pessoal.
