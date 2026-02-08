# 📱 Dashboard de Eficiência Mobile: Android vs. iOS

![Status do Projeto](https://img.shields.io/badge/Status-Conclu%C3%ADdo-brightgreen)
![Ferramenta](https://img.shields.io/badge/Ferramenta-Power%20BI-yellow)

## 📝 Descrição do Projeto
Este dashboard foi desenvolvido para analisar o comportamento de usuários de smartphones, focando na relação entre o **tempo de uso**, **tempo de tela (Screen On Time)** e o **consumo de bateria**. O objetivo é identificar padrões de eficiência energética entre os sistemas operacionais Android e iOS, além de segmentar o comportamento por perfis de uso (Leve, Moderado, Intenso, etc.).

## 🚀 Funcionalidades
* **Análise de KPIs:** Visualização rápida da média de idade, tempo de uso e drenagem de bateria.
* **Perfil de Usuário:** Gráfico de rosca segmentando a base de dados por classes de comportamento.
* **Comparativo de Gênero:** Análise de tempo de uso médio entre homens e mulheres em cada sistema operacional.
* **Correlação Técnica:** Gráfico de dispersão relacionando o tempo de tela com o gasto real de mAh.
* **Detalhamento:** Matriz completa para consulta de valores exatos por sistema.

## 📊 Insights Extraídos
* **Uso por Sistema:** Usuários de iOS apresentaram uma média de tempo de uso ligeiramente superior à do Android no dataset analisado.
* **Eficiência Energética:** A correlação entre tempo de tela e dreno de bateria é quase linear, mas perfis "Extremos" mostram uma inclinação maior de consumo, indicando menor eficiência em altas cargas.
* **Demografia:** O equilíbrio entre os gêneros no uso de dispositivos é consistente, com variações mínimas entre os sistemas operacionais.

## 🛠️ Tecnologias Utilizadas
* **Power BI:** Modelagem de dados e visualização.
* **Power Query:** Limpeza e transformação de dados (ETL).
* **DAX:** Criação de medidas calculadas e KPIs dinâmicos.
* **Dataset:** Dados de comportamento de uso mobile.

## ⚙️ Processamento e Transformação de Dados (ETL)
Para garantir a integridade das análises e o visual *clean* do dashboard, realizei as seguintes etapas no **Power Query**:

* **Normalização de Tipos:** Conversão rigorosa de colunas de consumo e tempo para formatos numéricos e decimais.
* **Renomeação Estratégica:** Simplificação de nomes técnicos (ex: `Battery Drain (mAh/day)`) para nomes amigáveis (ex: `Consumo de Bateria`), otimizando o espaço no layout mobile.
* **Criação de Colunas Condicionais:** Implementação da lógica de `User Behavior Class` para segmentar usuários em categorias baseando-se no volume de dados e tempo de tela.
* **Tratamento de Medidas (DAX):** * Criação de medidas de Média para suavizar as comparações.
    * Cálculo de KPIs dinâmicos sensíveis aos filtros de Sistema Operacional.
 
## Resultado
![Display celular](https://github.com/stephaniesouza25/PowerBI/blob/main/Mobile%20Behavior%20Analytics/Layout%20An%C3%A1lise.png)

## 📂 Como Visualizar este Projeto
1. Faça o download do arquivo `.pbix` presente neste repositório.
2. Abra no **Power BI Desktop**.
3. Caso os dados não carreguem, verifique o caminho da fonte de dados nas configurações do Power Query.

---
*Projeto desenvolvido para fins de estudo e análise de dados mobile.*
