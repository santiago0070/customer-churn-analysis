🟢 ETAPA 1: CONTEXTUALIZAÇÃO (Branding & Storytelling)
Universo do Projeto: ConnectPlus Telecom, uma provedora regional de serviços de internet e telefonia enfrentando alta competitividade.

Identidade Visual: Paleta Dark Mode & High Contrast. Fundo em cinza escuro (#121212), com Churn destacado em Coral/Laranja (#FF7F50) e Retenção em Turquesa (#40E0D0).

Business Case: A empresa identificou uma taxa de evasão crítica. O custo de aquisição de cliente (CAC) está subindo, tornando a retenção da base atual a prioridade estratégica para o Q3. O projeto visa identificar o perfil do cliente propenso ao cancelamento para ações de CRM preventivas.

🔵 ETAPA 2: ENGENHARIA DE DADOS (ETL & Coding)
Tratamento Técnico: * Limpeza de valores nulos e conversão de tipos (ex: TotalCharges para float).

Tratamento de outliers em MonthlyCharges.

Feature Engineering: Categorização de Tenure (tempo de casa) para identificar janelas críticas de saída.

KPIs & Regras:

Churn Rate (%): Razão entre clientes que saíram e o total da base.

Ticket Médio vs. Risco: Correlação entre cobranças elevadas e probabilidade de churn.

LTV (Lifetime Value) Estimado: Baseado no Tenure e MonthlyCharges.

🟡 ETAPA 3: BUSINESS INTELLIGENCE (Dashboarding)
Modelagem: Star Schema simples com Tabela Fato (Contratos) e Dimensões (Calendário, Serviços e Clientes).

Hierarquia de Telas:

Executivo: Visão macro de perda financeira mensal e taxa de churn atual.

Operacional: Filtros por tipo de contrato (Month-to-month) e método de pagamento para listas de repatriação.

UI/UX: Uso de análise de densidade (histogramas) para mostrar que o churn se concentra nos primeiros 10 meses de contrato, direcionando o olhar do analista para a "curva de perigo".

🟠 ETAPA 4: DOCUMENTAÇÃO TÉCNICA (GitHub)
Estrutura sugerida:

Plaintext
1. data/               # Datasets brutos e processados
2. notebooks/          # Churn_analise.ipynb
3. reports/            # Exportação dos gráficos em PNG/PDF
4. src/                # Scripts .py para automação do ETL
5. README.md           # Documentação Master

Trecho do README Master:

Análise de Churn Prediction - Telecom
Este projeto analisa os fatores determinantes para a evasão de clientes. Através de EDA (Exploratory Data Analysis), identificamos que contratos mensais associados ao método de pagamento Electronic Check possuem uma taxa de cancelamento 4x superior aos contratos anuais.

Principais Insights:

Janela Crítica: Clientes nos primeiros 6 meses de contrato exigem onboarding intensivo.

Sensibilidade a Preço: O Churn acentua-se em mensalidades acima de 80 unidades monetárias.
