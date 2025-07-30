# 📊 Telecom X – Parte 2: Prevendo Churn

Projeto desenvolvido como parte da Formação em Estatística e Machine Learning da Alura.

## 🎯 Descrição do Desafio

Após o sucesso na análise exploratória da evasão de clientes da Telecom X, fui convidada a integrar a equipe de Machine Learning da empresa. Nesta nova fase, a missão é construir modelos preditivos capazes de prever a evasão de clientes (churn), ajudando a empresa a agir preventivamente e reter sua base.

---

## 🧠 Objetivos

- ✅ Preparar os dados para modelagem (tratamento, codificação, normalização).
- ✅ Analisar correlações e realizar seleção de variáveis.
- ✅ Treinar modelos de classificação (Regressão Logística e Random Forest).
- ✅ Avaliar os modelos usando métricas apropriadas.
- ✅ Interpretar resultados, incluindo a importância das variáveis.
- ✅ Comunicar os principais fatores de evasão com sugestões estratégicas.

---

## 🧰 Tecnologias e Bibliotecas Utilizadas

- Python 3
- Pandas
- Scikit-learn
- Matplotlib / Seaborn (opcional para visualizações)
- Jupyter Notebook

---

## 🗂️ Estrutura do Projeto

```text
📁 telecom-x-parte-2/
├── dados_tratados.csv              # Base limpa e tratada (Parte 1)
├── telecom_churn_modelagem.ipynb   # Notebook com a modelagem e análises
├── README.md                       # Este arquivo
```
## 📌 Principais Etapas

1. **Carregamento e Pré-processamento**
   - Remoção de colunas irrelevantes como `ID_Cliente`.
   - Aplicação de One-Hot Encoding nas variáveis categóricas.
   - Verificação do balanceamento da variável alvo `Evasao`.

2. **Separação de Variáveis**
   - `X`: variáveis explicativas.
   - `y`: variável alvo (`Evasão`).

3. **Treinamento dos Modelos**
   - Regressão Logística com `StandardScaler` via pipeline.
   - Random Forest Classifier sem necessidade de normalização.

4. **Avaliação dos Modelos**
   - Matriz de confusão.
   - Relatório de classificação (precision, recall, f1-score, accuracy).

5. **Importância das Variáveis (Random Forest)**
   - Top 5 variáveis mais relevantes:
     - `Gasto_Total`
     - `Meses_Contrato`
     - `Gasto_Mensal`
     - `Gasto_Diario`
     - `Tipo_Contrato_Mês a mês`

## 📈 Conclusões e Estratégias

Com base nos resultados:

- Clientes com maior gasto total, planos mensais e curta duração de contrato apresentam maior chance de evasão.

A empresa deve:

- Incentivar migração para contratos anuais.
- Criar ofertas customizadas para clientes com altos gastos.
- Implementar ações preventivas nos primeiros meses de contrato.

## 👩‍💻 Autoria

Projeto desenvolvido por **Allie**  
Formação: **Estatística e Machine Learning – Alura**
