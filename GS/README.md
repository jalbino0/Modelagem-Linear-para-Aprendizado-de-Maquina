# 📊 Classificação de Vagas por Nível (Junior vs Senior)

Este projeto utiliza **Machine Learning** para classificar vagas de emprego como **Junior** ou **Senior** com base nas **skills exigidas**, utilizando Python e regressão logística.

---

## 📂 Arquivos Necessários

- `job_postings.csv` → informações das vagas  
- `job_skills.csv` → lista de skills associadas às vagas  

Os arquivos são unidos pela coluna `job_link`.

---

## 🎯 Objetivo

Criar um modelo de classificação binária capaz de prever o **nível da vaga** (Junior ou Senior) a partir das skills descritas, além de identificar quais habilidades mais influenciam cada nível.

---

## 🛠️ Tecnologias Utilizadas

- Python  
- Pandas  
- NumPy  
- Scikit-learn  

---

## ⚙️ Etapas do Código

1. **Carregamento dos dados**  
   Leitura dos arquivos CSV e verificação do formato.

2. **Merge e limpeza**  
   União dos datasets e remoção de valores nulos.

3. **Criação da variável alvo**  
   - Associate → Junior (0)  
   - Mid senior → Senior (1)

4. **Pré-processamento das skills**  
   Transformação das skills em texto utilizando **TF-IDF**.

5. **Treinamento do modelo**  
   Aplicação de **Regressão Logística** com balanceamento de classes.

6. **Avaliação do modelo**  
   - Acurácia  
   - Relatório de classificação  
   - Matriz de confusão  

7. **Interpretação dos resultados**  
   Identificação das skills que mais aumentam a probabilidade de uma vaga ser Junior ou Senior.

---

## ▶️ Como Executar

1. Certifique-se de ter os arquivos CSV na mesma pasta do código.
2. Instale as dependências:
   ```bash
   pip install pandas numpy scikit-learn
