# 📊 Customer Churn Analysis

## 🎯 Objetivo
Analisar dados de clientes para identificar padrões de churn (cancelamento) e gerar insights que apoiem estratégias de retenção.

---

## 📌 Contexto de Negócio
O churn de clientes representa perda direta de receita para empresas.  
Entender os fatores que levam ao cancelamento permite ações mais eficientes de retenção e melhoria da experiência do cliente.

---

## 🛠️ Tecnologias Utilizadas

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 📂 Estrutura do Projeto
customer-churn-analysis
┣ 📄 churn_analysis.ipynb
┣ 📁 data/
┗ 📄 README.md

---

## 🔍 Etapas da Análise

### 1. Tratamento de Dados
- Remoção de valores nulos
- Conversão de tipos de dados
- Padronização das colunas

---

### 2. Análise Exploratória (EDA)
- Distribuição de clientes por churn
- Análise por tipo de contrato
- Tempo de permanência (tenure)
- Valor mensal (Monthly Charges)
- Métodos de pagamento

---

### 3. Análise de Métricas
- Taxa geral de churn

---

## 📊 Principais Insights

- Clientes com contrato **mensal** apresentam maior taxa de churn  
- Clientes com **baixo tempo de permanência** têm maior probabilidade de cancelamento  
- Cobranças mensais mais altas indicam tendência ao churn  
- O início do ciclo de vida do cliente é o momento mais crítico para retenção  

---

## ⚠️ Identificação de Risco

Foi criada uma lógica simples para identificar clientes com maior risco de churn:

- Contrato mensal  
- Tempo de permanência inferior a 12 meses  

Essa abordagem permite direcionar ações preventivas de retenção.

---

## 🚀 Conclusão

A análise demonstra que estratégias de retenção devem focar principalmente em:

- Clientes novos  
- Clientes com contrato mensal  

A utilização de dados permite antecipar comportamentos e reduzir perdas de clientes.

---

## 👨‍💻 Autor

Rodrigo Santiago  
🔗 LinkedIn: www.linkedin.com/in/r0drig0-santiag0
📧 Email: rodrigow9191@gmail.com
