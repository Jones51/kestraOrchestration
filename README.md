# Orquestração de Dados com Kestra

## 🛠️ Introdução 
Este projeto prático demonstra a capacidade de orquestração de dados de ponta a ponta utilizando Kestra, uma poderosa plataforma open-source. O foco é simular um cenário de integração de dados complexa e em paralelo proveniente de múltiplas APIs externas. O pipeline desenvolvido realiza o consumo simultâneo desses dados, aplica transformações e gerencia o armazenamento em diferentes sistemas de banco de dados (PostgreSQL e MongoDB), consolidando informações para uso analítico ou de aplicação.

## 📝 Problema de Negócios 
O desafio de negócio abordado é a centralização e harmonização de dados provenientes de fontes heterogêneas e distribuídas (duas APIs distintas). Em um contexto empresarial, a tomada de decisão precisa de uma visão unificada que não pode ser alcançada se os dados estiverem isolados e em formatos incompatíveis. O problema técnico é a necessidade de uma solução robusta para orquestrar o consumo paralelo dessas fontes, garantir a integridade e consistência na ingestão no PostgreSQL, realizar a combinação e transformação necessárias e, finalmente, consolidar os resultados em um datastore moderno (MongoDB) para consumo rápido e escalável.

## 🎓 Metodologia 
A metodologia utilizada baseia-se na implementação de um Pipeline de Dados Orquestrado dentro do Kestra, seguindo os princípios de um processo ETL (Extract, Transform, Load).

Extração Paralela (E): Duas tarefas no Kestra foram configuradas para consumir dados de APIs distintas simultaneamente, maximizando a eficiência e reduzindo a latência do pipeline.

Carga Intermediária (L): Os dados extraídos foram armazenados em um banco de dados PostgreSQL, servindo como staging area e garantindo a persistência dos dados brutos/semi-brutos antes da consolidação final.

Transformação e Combinação (T): Utilizando funcionalidades do Kestra e/ou código customizado (por exemplo, Python ou SQL), os dados do PostgreSQL foram combinados e transformados em um esquema unificado.

Carga Final (L): Os dados transformados e consolidados foram inseridos em um banco de dados MongoDB, ideal para servir a aplicações que exigem flexibilidade de esquema ou alta performance de leitura.

Orquestração: Todo o fluxo foi gerenciado pelo Kestra, utilizando triggers para automação e monitoramento para garantir a execução bem-sucedida e a manipulação de falhas.

<img width="1342" height="376" alt="image" src="https://github.com/user-attachments/assets/5d1789af-e0d3-4236-8fbe-7957e53c380c" />


## 📊 Habilidades 
Orquestração de Workflows: Domínio da plataforma Kestra para projetar, construir e monitorar fluxos de trabalho complexos e paralelos.

Integração de APIs: Habilidade em consumir e manipular dados de APIs RESTful externas.

Bancos de Dados Relacionais: Conhecimento prático em PostgreSQL, incluindo ingestão de dados e execução de consultas para combinação de datasets.

Bancos de Dados NoSQL: Experiência com MongoDB para o armazenamento final e consolidação de dados estruturados e semi-estruturados.

Processamento Paralelo: Capacidade de configurar tarefas para execução simultânea, otimizando o tempo de processamento do pipeline.

Data Engineering Fundamentals: Entendimento de conceitos de ETL, staging de dados e data warehousing em um contexto de modern data stack.

Pipeline as Code: Habilidade em definir fluxos de trabalho de dados de forma declarativa e automatizada.

## 🪄 Projeto Final 
<img width="1865" height="201" alt="image" src="https://github.com/user-attachments/assets/a4571c70-66f6-495c-8f29-6d49e1ffaaaf" />

<img width="1773" height="838" alt="image" src="https://github.com/user-attachments/assets/2bf4502f-514f-4e5f-8138-86b7f307e2c6" />













