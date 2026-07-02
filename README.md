# 🩺 Predição de Obesidade com Machine Learning

<div align="center">

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange?logo=scikitlearn)
![Streamlit](https://img.shields.io/badge/Streamlit-App-red?logo=streamlit)
![Status](https://img.shields.io/badge/Status-Concluído-success)

### Tech Challenge • Pós-Tech FIAP • Data Analytics - Fase 4

</div>

---

# 📌 Sobre o Projeto

Este projeto foi desenvolvido como parte do **Tech Challenge – Fase 4** da Pós-Tech em Data Analytics (FIAP).

O desafio consiste em construir uma solução completa baseada em **Machine Learning** capaz de auxiliar equipes médicas na identificação do nível de obesidade de um paciente utilizando informações físicas, hábitos alimentares e estilo de vida.

Além do treinamento do modelo, o projeto contempla todo o fluxo de Ciência de Dados, desde a exploração da base até a disponibilização do modelo para inferência.

---

# 🎯 Objetivos

- Desenvolver uma pipeline completa de Machine Learning.
- Realizar Engenharia de Features.
- Comparar diferentes algoritmos de classificação.
- Selecionar o modelo com melhor capacidade de generalização.
- Persistir o modelo treinado.
- Disponibilizar uma aplicação utilizando Streamlit.
- Gerar insights para apoio à tomada de decisão médica.

---

# 📊 Dataset

A base utilizada contém informações relacionadas aos hábitos de vida dos pacientes.

## Variáveis

| Categoria | Variáveis |
|------------|-----------|
| Perfil | Gender, Age |
| Medidas Corporais | Height, Weight |
| Alimentação | FCVC, NCP, CAEC, FAVC |
| Saúde | CH2O, SCC, FAF |
| Hábitos | SMOKE, CALC |
| Mobilidade | MTRANS |
| Histórico | family_history |
| Variável alvo | Obesity |

---

# 🏗 Arquitetura do Projeto

```
                 Dataset
                    │
                    ▼
          Análise Exploratória
                    │
                    ▼
        Engenharia de Features
                    │
                    ▼
      Pré-processamento dos Dados
                    │
                    ▼
      Pipeline de Machine Learning
                    │
         ┌──────────┴──────────┐
         ▼                     ▼
   Treinamento          Validação
         │
         ▼
 Comparação de Modelos
         │
         ▼
 Seleção do Melhor Modelo
         │
         ▼
      hgb.joblib
         │
         ▼
 Aplicação Streamlit
```

---

# 📂 Estrutura do Projeto

```
.
├── model.ipynb              # Desenvolvimento completo do projeto
├── Obesity.csv              # Base de dados
├── hgb.joblib               # Modelo treinado
├── requirements.txt
├── README.md
```

---

# 🔍 Análise Exploratória

Durante a etapa exploratória foram realizadas análises como:

- Distribuição das classes
- Estatísticas descritivas
- Verificação de valores ausentes
- Correlação entre variáveis
- Distribuição das variáveis categóricas
- Avaliação da qualidade da base

---

# ⚙️ Engenharia de Features

Foram aplicadas técnicas de preparação dos dados, incluindo:

- Remoção de atributos com baixa contribuição
- Codificação de variáveis categóricas
    - One-Hot Encoding
    - Ordinal Encoding
    - Label Encoding
- Construção da Pipeline
- Balanceamento das classes utilizando Oversampling
- Separação entre treino e teste

---

# 🤖 Modelos Avaliados

Foram comparados diversos algoritmos supervisionados de classificação.

- Decision Tree
- Random Forest
- Extra Trees
- HistGradientBoosting
- XGBoost
- Logistic Regression
- Outros modelos avaliados durante os experimentos

A seleção do modelo foi baseada na capacidade de generalização e não apenas na maior acurácia.

---

# 📈 Métricas Utilizadas

Como o problema possui **7 classes**, foram utilizadas métricas específicas para classificação multiclasse.

- Accuracy
- Balanced Accuracy
- Precision Macro
- Recall Macro
- F1-Score Macro
- ROC AUC OvR
- KS Statistic OvR
- Matriz de Confusão

---

# 🧪 Pipeline de Machine Learning

A solução contempla todas as etapas do treinamento:

- Importação dos dados
- Limpeza
- Engenharia de atributos
- Codificação das variáveis
- Balanceamento
- Split Treino/Teste
- Construção da Pipeline
- Treinamento
- Validação
- Avaliação
- Exportação do modelo

---

# 💾 Modelo Final

Após a comparação entre os algoritmos foi selecionado o modelo com melhor desempenho e capacidade de generalização.

O modelo treinado encontra-se salvo em:

```
hgb.joblib
```

---

# 🚀 Como executar

Clone o projeto

```bash
git clone https://github.com/seuusuario/tech-challenge-fase4.git
```

Entre na pasta

```bash
cd tech-challenge-fase4
```

Crie um ambiente virtual

```bash
python -m venv venv
```

Ative

Windows

```bash
venv\Scripts\activate
```

Linux/Mac

```bash
source venv/bin/activate
```

Instale as dependências

```bash
pip install -r requirements.txt
```

Execute o Notebook

```bash
jupyter notebook
```

Ou execute a aplicação

```bash
streamlit run app.py
```

---

# 📊 Resultados

O projeto atingiu os requisitos propostos pelo desafio.

✔ Pipeline completa de Machine Learning

✔ Engenharia de Features

✔ Avaliação de múltiplos modelos

✔ Modelo com desempenho superior ao mínimo exigido

✔ Persistência do modelo treinado

✔ Preparação para Deploy com Streamlit

---

# 🛠 Tecnologias

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-Learn
- Imbalanced-Learn
- Joblib
- Streamlit
- Jupyter Notebook

---

# 📚 Requisitos do Desafio

- ✔ Pipeline completa de Machine Learning
- ✔ Feature Engineering
- ✔ Modelo com assertividade superior a 75%
- ✔ Aplicação preditiva
- ✔ Dashboard analítico
- ✔ Deploy
- ✔ Repositório GitHub

---

# 📖 Referência

Projeto desenvolvido como requisito do **Tech Challenge – Fase 4** da Pós-Tech em Data Analytics, cujo objetivo é construir uma solução preditiva para auxiliar profissionais da saúde na classificação do nível de obesidade de pacientes. :contentReference[oaicite:1]{index=1}

---

# 👨‍💻 Autor

**Renato Moschetta**

Especialista em Engenharia de Software • Machine Learning • Data Analytics

GitHub: https://github.com/SEU_USUARIO

LinkedIn: https://linkedin.com/in/SEU_USUARIO

---

## ⭐ Se este projeto foi útil para você, deixe uma estrela no repositório.
