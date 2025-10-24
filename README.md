# 🚀 Modelo Estrela com Power BI – Análise de Vendas e Performance Comercial

Este projeto foi desenvolvido com o objetivo de transformar o conjunto de dados *Financials Sample* em um modelo dimensional robusto, utilizando o Power BI como plataforma de análise. Partindo de uma única tabela, foi estruturado um **modelo estrela completo**, com tabelas fato e dimensão que permitem explorar insights estratégicos sobre vendas, produtos, descontos e sazonalidade.

<img width="1395" height="779" alt="Página 1 - DB" src="https://github.com/user-attachments/assets/2d6d0256-0963-4777-b285-6fc64dbdee5b" />
<img width="1395" height="779" alt="Página 2 - DB" src="https://github.com/user-attachments/assets/a5340769-f473-439e-b656-25b064c965a4" />
<img width="1194" height="848" alt="StarSchemaCriado" src="https://github.com/user-attachments/assets/9a56ce92-bd48-499d-a351-0edf7cac9d89" />



## 🧠 Motivação

Em vez de trabalhar com uma tabela única e plana, optei por aplicar técnicas de modelagem dimensional para melhorar a performance das análises e facilitar a criação de medidas DAX. O resultado é um modelo limpo, escalável e pronto para responder perguntas de negócio com agilidade.

## 🧱 Estrutura do Modelo

O modelo foi construído com base em relacionamentos bem definidos entre as tabelas, conforme o esquema estrela abaixo:

### 🔸 Tabela Fato

- **F_Vendas**: Contém os dados transacionais, como produto, unidades vendidas, valor de venda, lucro, faixa de desconto, segmento, país, vendedor e data.

### 🔹 Tabelas Dimensão

- **D_Produtos**: Agrega estatísticas por produto, como média, mediana, mínimo e máximo de vendas.
- **D_Produtos_Detalhes**: Traz informações técnicas como preço de fabricação, faixa de desconto e preço de venda.
- **D_Descontos**: Mapeia faixas de desconto e percentuais aplicados.
- **D_Categoria**: Segmenta os dados por país, segmento e índice de categorização.
- **D_Calendar**: Criada com `CALENDAR()` e enriquecida com campos como trimestre e dia da semana.

## 📊 Dashboards Criados

O projeto inclui dois painéis principais:

### 1. **Desempenho por Produto**
- Identifica o produto mais vendido (`Paseo`), a categoria com maior lucro (`Government`) e a faixa de desconto mais usada (`Medium`).
- Gráficos de barras e rosca mostram unidades vendidas e média de lucro por produto.

### 2. **Resumo Comercial**
- Métricas agregadas: lucro total, vendas totais, unidades vendidas.
- Gráficos de vendas por dia da semana, lucro por trimestre e distribuição de vendas por produto.
- Destaque para o **T4** como trimestre com maior volume de vendas.

## ⚙️ Técnicas Utilizadas

- **Modelagem Dimensional**: Separação clara entre fatos e dimensões.
- **DAX Avançado**: Uso de funções como `CALCULATE`, `SUMX`, `MEDIANX`, `RELATED`, `SWITCH`, entre outras.
- **Criação de Índices**: Lógica condicional para categorização de produtos e segmentos.
- **Visualizações Interativas**: Dashboards intuitivos e responsivos, com foco em usabilidade.

## 💡 Conclusão

Este projeto demonstra como é possível transformar um dataset simples em uma estrutura analítica poderosa. A modelagem em estrela não só melhora a performance, como também organiza o raciocínio analítico. É uma vitrine de boas práticas em Power BI, voltada para quem busca entregar valor com dados.
