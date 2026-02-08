📱 Dashboard de Eficiência Mobile: Android vs. iOS
📝 Descrição do Projeto
Este dashboard foi desenvolvido para analisar o comportamento de usuários de smartphones, focando na relação entre o tempo de uso, tempo de tela (Screen On Time) e o consumo de bateria. O objetivo é identificar padrões de eficiência energética entre os sistemas operacionais Android e iOS, além de segmentar o comportamento por perfis de uso (Leve, Moderado, Intenso, etc.).

🚀 Funcionalidades
Análise de KPIs: Visualização rápida da média de idade, tempo de uso e drenagem de bateria.

Perfil de Usuário: Gráfico de rosca segmentando a base de dados por classes de comportamento.

Comparativo de Gênero: Análise de tempo de uso médio entre homens e mulheres em cada sistema operacional.

Correlação Técnica: Gráfico de dispersão relacionando o tempo de tela com o gasto real de mAh.

Detalhamento: Matriz completa para consulta de valores exatos por sistema.

📊 Insights Extraídos (Exemplos)
Usuários de iOS apresentaram uma média de tempo de uso ligeiramente superior à do Android no dataset analisado.

A correlação entre tempo de tela e dreno de bateria é quase linear, mas perfis "Extremos" mostram uma inclinação maior de consumo.

O equilíbrio entre os gêneros no uso de dispositivos é consistente, com pequenas variações dependendo do sistema operacional.

🛠️ Tecnologias Utilizadas
Power BI: Tratamento de dados (Power Query), modelagem e visualização.

DAX: Criação de medidas de média e contagem para os KPIs.

Dataset: Dados simulados/reais de comportamento mobile.

🛠️ Processamento e Transformação de Dados (ETL)
Para garantir a integridade das análises e o visual "clean" do dashboard, realizei as seguintes etapas no Power Query:

Normalização de Tipos: Conversão rigorosa de colunas de consumo e tempo para formatos numéricos e decimais para cálculos precisos de média.

Renomeação Estratégica: Simplificação de nomes de colunas técnicos (ex: Battery Drain (mAh/day)) para nomes amigáveis ao usuário final (ex: Consumo de Bateria), otimizando o espaço no layout mobile.

Criação de Colunas Condicionais: Implementação da lógica de User Behavior Class para segmentar usuários em categorias (Leve, Moderado, Intenso, Extremo) baseando-se no volume de dados e tempo de tela.

Tratamento de Medidas (DAX): * Criação de medidas de Média Móvel para suavizar as comparações entre sistemas operacionais.

Cálculo de KPIs dinâmicos que respondem instantaneamente aos filtros de Sistema Operacional.

📂 Como Visualizar este Projeto
Faça o download do arquivo .pbix presente neste repositório.

Abra no Power BI Desktop.

Caso os dados não carreguem, verifique o caminho da fonte de dados no Power Query.