# Churn_telecom
Modelo de Churn
# Data_Analytics
## Projeto de Análise de Churn em Telecomunicações com Power BI

Este projeto tem como objetivo analisar o churn em uma empresa de telecomunicações usando o Power BI. O churn refere-se à taxa de perda de clientes ao longo do tempo e é um fator crítico para a lucratividade das empresas de telecomunicações.

# Dicionario de Dados:
Churn Label: Sim = o cliente saiu da empresa neste trimestre. Não = o cliente permaneceu na empresa. Diretamente relacionado ao Churn Value.
Churn Value: 1 = o cliente saiu da empresa neste trimestre. 0 = o cliente permaneceu na empresa. Diretamente relacionado ao Churn Label.
Churn Score: Um valor de 0 a 100 que é calculado usando a ferramenta preditiva IBM SPSS Modeler. O modelo incorpora vários fatores conhecidos por causar churn. Quanto maior a pontuação, maior a probabilidade de rotatividade do cliente.
CLTV: valor vitalício do cliente. Um CLTV previsto é calculado usando fórmulas corporativas e dados existentes. Quanto maior o valor, mais valioso o cliente. Clientes de alto valor devem ser monitorados quanto ao churn.
Churn Reason: Razão específica de um cliente para deixar a empresa. Diretamente relacionado à categoria Churn.
Contract: Indica o tipo de contrato atual do cliente: Mês a Mês, Um Ano, Dois Anos.
CustomerID: Um ID exclusivo que identifica cada cliente.
Count: um valor usado em relatórios/painéis para somar o número de clientes em um conjunto filtrado.
Country: o país de residência principal do cliente.
City: a cidade da residência principal do cliente.
Dependents: Indica se o cliente mora com algum dependente: Sim, Não. Os dependentes podem ser filhos, pais, avós, etc.
Device Protection Plan: Indica se o cliente assina um plano de proteção de dispositivo adicional para seu equipamento de Internet fornecido pela empresa: Sim, Não
Gender: Sexo do cliente: Masculino, Feminino
Internet Service: Indica se o cliente assina serviço de Internet com a empresa: Não, DSL, Fibra Óptica, Cabo.
Lat Long: a latitude e longitude combinadas da residência principal do cliente.
Latitude: a latitude da residência principal do cliente.
Longitude: a longitude da residência principal do cliente.
Married: Indica se o cliente é casado: Sim, Não
Multiple Lines: Indica se o cliente assina várias linhas telefônicas com a empresa: Sim, Não
Monthly Charge: Indica a cobrança mensal total atual do cliente para todos os seus serviços da empresa.
Online Security: Indica se o cliente subscreve um serviço adicional de segurança online disponibilizado pela empresa: Sim, Não
Online Backup: Indica se o cliente subscreve um serviço adicional de backup online disponibilizado pela empresa: Sim, Não
Premium Tech Support: Indica se o cliente subscreve um plano de suporte técnico adicional da empresa com tempos de espera reduzidos: Sim, Não
Phone Service: Indica se o cliente subscreve o serviço telefónico domiciliário da empresa: Sim, Não 
Paperless Billing: Indica se o cliente optou pelo faturamento sem papel: Sim, Não
Payment Method: Indica como o cliente paga sua fatura: Boleto Bancário, Cartão de Crédito, Cheque Postado
Senior Citizen: Indica se o cliente tem 65 anos ou mais: Sim, Não
State: O estado da residência principal do cliente.
Streaming TV: Indica se o cliente utiliza seu serviço de Internet para transmitir programação de televisão de um provedor terceirizado: Sim, Não. A empresa não cobra taxa adicional por este serviço.
Streaming Movies: Indica se o cliente utiliza seu serviço de Internet para streaming de filmes de um provedor terceirizado: Sim, Não. A empresa não cobra taxa adicional por este serviço.
Total Charges: Indica as cobranças totais do cliente, calculadas até o final do trimestre especificado acima.
Tenure in Months: Indica o total de meses que o cliente está na empresa até o final do trimestre especificado acima.
Zip Code: O CEP da residência principal do cliente.

# Preparação dos Dados
A maioria dos tratamentos dos dados foi realizada com o uso do Power Query Editor, ferramenta para preparar e tratar o dado no Power BI.

# Tratamentos dos Dados no Power Query Editor
Abaixo seguem os tratamentos realizados:

Criação do grupo "Churn Score (grupos)" a partir da coluna "churn Score" para segmentação por grupos dos clientes de acordo com a pontuação de cada um.

Criação do grupo "CLTV (grupos)" a partir das colunas "CLTV" para distribuir a pontuação de acordo com o valor de cada cliente. Foi utilizada a métrica: Ouro, Prata e Bronze para segmentação.

Criação da coluna "Total Servicos Subscritos" para resumir o numero de serviços que cada cliente possui, já que essa informação apenas era encontrada em cada coluna de serviço como "sim" ou "nao".

Criação de várias "#Medidas" utilizadas para geração do Dashboard.

# Contribuições
Contribuições e sugestões são bem-vindas! Fique à vontade para abrir problemas (issues) ou enviar solicitações de pull (pull requests) para melhorar este projeto.

Veja o arquivo de dados em 
www.kaggle.com/datasets/yeanzc/telco-customer-churn-ibm-dataset/Projeto_MAchine_Learning.ipynb

Agradecemos a IBM Cognos Analytics por disponibilizar o conjunto de dados.
