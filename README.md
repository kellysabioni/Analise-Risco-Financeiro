# Sistema Inteligente de Análise de Perfil Financeiro

## Sobre o Projeto

Este projeto foi desenvolvido como proposta de conclusão do Hackathon de Dados, com foco no tema **Risk Intelligence (Risco Financeiro)**.

A solução tem como objetivo analisar padrões financeiros e identificar possíveis comportamentos de risco utilizando:

- Engenharia e tratamento de dados
- Estatística exploratória
- SQL para consultas analíticas
- Machine Learning para previsão de risco
- Dashboards analíticos em Power BI
- Geração de insights estratégicos para tomada de decisão

O projeto simula um fluxo completo de dados, desde a ingestão até a geração de previsões e visualizações executivas.

---

# Objetivo

Desenvolver um sistema inteligente capaz de:

- Detectar comportamentos financeiros fora do padrão
- Gerar um score de risco financeiro
- Apoiar decisões estratégicas com dados
- Transformar dados brutos em insights acionáveis
- Demonstrar um pipeline completo de Data Analytics + Machine Learning

---

# Tema Escolhido — Risk Intelligence

## Foco

Identificação de risco financeiro através da análise de transações e comportamento de consumo.

## Problema Resolvido

Instituições financeiras precisam identificar rapidamente:

- Clientes com comportamento de risco
- Possíveis fraudes ou anomalias
- Uso excessivo de limite
- Padrões financeiros incomuns
- Perfis com maior probabilidade de inadimplência

O sistema proposto automatiza essa análise utilizando técnicas estatísticas e modelos preditivos.

---

# Arquitetura da Solução

```text
Dados CSV / Banco de Dados
           ↓
Extração e Limpeza dos Dados
           ↓
Análise Exploratória (Python + Estatística)
           ↓
Feature Engineering
           ↓
Treinamento de Modelos de Machine Learning
           ↓
Geração do Score de Risco
           ↓
Exportação dos Dados Tratados
           ↓
Dashboard Power BI
           ↓
Insights Estratégicos
```

---

# Tecnologias Utilizadas

## Linguagens e Ferramentas

- Python
- SQL
- Power BI
- Google Colab
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn
- PySpark
- Imbalanced-Learn (SMOTE)

---

# Estrutura do Projeto

```text
📁 projeto-risk-intelligence
│
├── 📄 README.md
├── 📄 ML_Risco_Financeiro_Tema3.ipynb
├── 📄 ML_06.csv
├── 📄 risco_financeiro_com_score.csv
├── 📄 resumo_por_nivel_risco.csv
├── 📁 sql
│   └── queries.sql
```

---

# Etapas do Projeto

## Coleta e Preparação dos Dados

Os dados financeiros foram carregados a partir de arquivos CSV.

Durante essa etapa foram realizados:

- Tratamento de valores nulos
- Padronização de dados
- Conversão de tipos
- Amostragem estratificada (300k linhas de 8,9 milhões)
- Limpeza de inconsistências

---

## Análise Exploratória de Dados (EDA)

Foram aplicadas análises estatísticas e visuais para compreender:

- Distribuição dos clientes de risco
- Relação entre limite e gastos
- Padrões de transações
- Horários de maior incidência de risco
- Comportamento financeiro por perfil

### Principais análises realizadas

- Distribuição do target
- Histogramas
- Boxplots
- Heatmap de correlação
- Análise temporal
- Estatística descritiva

---

# Engenharia de Features

Foram criadas variáveis derivadas para melhorar a capacidade preditiva do modelo.

## Exemplos

- Percentual do limite utilizado
- Faixa de gasto
- Indicadores temporais
- Relações entre saldo e transação

Essas features ajudaram o modelo a identificar padrões financeiros mais complexos.

---

# Machine Learning

## Modelos Utilizados

Foram treinados e comparados dois modelos:

### Random Forest

Modelo baseado em múltiplas árvores de decisão.

### Gradient Boosting

Modelo baseado em boosting para melhorar a performance preditiva.

---

## Balanceamento de Classes

Foi utilizada a técnica:

- SMOTE (Synthetic Minority Over-sampling Technique)

### Objetivo

Corrigir o desbalanceamento entre clientes de risco e não risco.

---

# Avaliação dos Modelos

Os modelos foram avaliados utilizando:

- Precision
- Recall
- F1-Score
- ROC-AUC
- Matriz de Confusão

Também foram geradas:

- Curvas ROC
- Comparações de performance
- Ranking de importância das features

---

# Score de Risco Financeiro

Após o treinamento, o melhor modelo foi utilizado para gerar:

- Probabilidade de risco
- Score financeiro
- Classificação de clientes

Os resultados foram exportados para utilização no dashboard e em análises futuras.

---

# Consultas SQL

O projeto também contempla consultas SQL para:

- Tratamento de dados nulos
- Análises segmentadas
- Estatísticas financeiras
- Extração de insights
- Agregações por categoria/região/perfil

---

# Principais Insights Obtidos

- Clientes com maior utilização do limite apresentaram maior risco financeiro
- Alguns horários do dia apresentaram maior incidência de transações suspeitas
- O comportamento de consumo possui forte relação com o score de risco
- Variáveis derivadas aumentaram significativamente a capacidade preditiva do modelo
- O balanceamento das classes melhorou a detecção de clientes críticos

---

# Possíveis Evoluções

- Deploy do modelo em API
- Atualização em tempo real dos scores
- Integração com banco de dados em nuvem
- Detecção automática de fraudes
- Sistema de alertas inteligentes
- Modelos mais avançados de Deep Learning

---

# Como Executar o Projeto

## 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/projeto-risk-intelligence.git
```

## 2. Instale as dependências

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn pyspark
```

## 3. Execute o notebook

Abra o arquivo:

```text
ML_Risco_Financeiro_Tema3.ipynb
```

no Google Colab ou Jupyter Notebook.

---

# Notebook Principal

## Google Colab — Sistema Inteligente de Risco Financeiro

https://colab.research.google.com/drive/1LGeweNQUS6gigcDWFXTquJAufIV6Bdkc?usp=sharing

---

# Equipe — Grupo 19

Projeto desenvolvido para o Hackathon de Dados.

## Integrantes

- Janyelle Oliveira Pinto de Castro — janyelleoliveira30@gmail.com
- Karen
- Kelly Cristina Sabioni — kelly.sabioni@yahoo.com.br
- Luma

---

# Resultado Esperado

Demonstrar uma solução completa de engenharia, análise e ciência de dados capaz de transformar informações financeiras em inteligência estratégica.

---

# Competências Aplicadas

✅ Python para análise de dados  
✅ Estatística exploratória  
✅ SQL para consultas analíticas  
✅ Storytelling com dados  
✅ Machine Learning supervisionado  
✅ Feature Engineering  
✅ Balanceamento de classes  
✅ Visualização de dados  
✅ Pipeline completo de Data Science


