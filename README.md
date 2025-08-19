# MVP2 - COVID19

Análise exploratória, pré-processamento e preparação de dados de um conjunto de pacientes com suspeita ou confirmação de COVID-19, com foco na investigação de fatores associados à mortalidade.

## 📌 Objetivo

Este projeto tem como objetivo principal realizar o pré-processamento e a análise exploratória de um dataset de pacientes com COVID-19, identificando padrões e relações entre comorbidades, faixa etária, internação e óbito. Ao final da análise, o conjunto de dados estará pronto para ser utilizado em modelos preditivos.

## 🧠 Hipóteses levantadas

- Existe relação entre idade e mortalidade por COVID-19?
- Comorbidades aumentam a chance de óbito?
- A intubação e o uso de UTI indicam maior gravidade e risco de morte?

## 🗃️ Fonte dos dados

- Dataset original disponível no Kaggle:  
  [COVID-19 Dataset - Meir Nizri](https://www.kaggle.com/datasets/meirnizri/covid19-dataset)

## ⚙️ Etapas realizadas

1. **Carregamento dos dados**
2. **Análise inicial e identificação de inconsistências**
3. **Tratamento de valores ausentes**
   - Comorbidades com nulos preenchidas com `0` (ausência da condição)
   - Coluna `pregnant` tratada com base no sexo do paciente
   - Criação de variável binária `died` a partir da `date_died`
4. **Conversão de variáveis**
   - Binárias transformadas para tipo `boolean`
   - Codificação de variáveis categóricas com One-Hot Encoding
5. **Criação de faixas etárias**
6. **Análise exploratória**
   - Gráficos de distribuição
   - Boxplots
   - Histogramas
   - Matrizes de correlação
7. **Preparação final dos dados para modelagem**

## 📊 Principais descobertas

- A mortalidade aumenta significativamente com a idade, principalmente acima dos 50 anos.
- Comorbidades como hipertensão, diabetes e DPOC estão fortemente associadas a óbitos.
- Intubação e internação em UTI também se relacionam com maior risco de morte.
- A maioria dos registros está concentrada em pacientes que não apresentam comorbidades, o que exigiu atenção no balanceamento e tratamento dos dados.

## 📁 Estrutura do projeto

## 🧪 Tecnologias utilizadas

- Python 3.10+
- Pandas
- NumPy
- Matplotlib / Seaborn

## ✍️ Autor

**Eduardo Camargo Ribeiro Borges**  
Pós-graduação em Ciência de Dados e Analytics  
PUC-RIO

---

> *Este projeto foi desenvolvido como parte da entrega do MVP2 da pós-graduação.*
