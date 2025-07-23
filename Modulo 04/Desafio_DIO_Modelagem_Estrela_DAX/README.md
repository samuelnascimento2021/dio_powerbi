# 📊 Projeto Power BI – Modelo Estrela com Tabela Financial Sample

Este projeto tem como objetivo aplicar os conceitos de modelagem dimensional utilizando Power BI, com foco na construção de um **esquema em estrela** (Star Schema) a partir da base de dados **Financial Sample**.

## 🧩 Estrutura do Projeto

A partir da tabela original `Financial Sample`, foram criadas:

### 🔷 Tabelas Dimensão

- **D_Produtos**: Contém produto, média de unidades vendidas, valores médios, mediana, máximo e mínimo de vendas.
- **D_Produtos_Detalhes**: Informações detalhadas como faixa de desconto, preço de venda, unidades vendidas e preço de fabricação.
- **D_Descontos**: Nível de desconto aplicado por produto.
- **D_Detalhes**: Tabela auxiliar com demais colunas informativas não aproveitadas nas outras dimensões.
- **D_Calendario**: Criada com DAX utilizando `CALENDARAUTO()` e enriquecida com colunas como ano, mês, nome do dia da semana e data formatada.

### 🔶 Tabela Fato

- **F_Vendas**: Centraliza as informações de vendas, como produto, quantidade vendida, preço, lucro, vendedor, país e data.

## 🛠️ Principais Técnicas Utilizadas

- **Criação de Tabelas com DAX**: `CALENDARAUTO()`, `ADDCOLUMNS()`, `SWITCH()`, `FORMAT()`
- **KPI por Agrupamento**: Média, mediana, máximo e mínimo via agregações DAX.
- **Relatórios Visuais**: Segmentações e painéis baseados na estrutura modelada.
- **Formatação Personalizada de Datas**: Formatação avançada para apresentar datas no padrão `segunda-feira, 1 de dezembro de 2014`.

## 📌 Etapas do Projeto

1. Criação das tabelas dimensão e fato a partir da base original.
2. Aplicação de transformações, agrupamentos e condições para enriquecer os dados.
3. Construção de relacionamentos no esquema estrela.
4. Criação de medidas DAX para análise.
5. Salvamento do arquivo `.pbix` e exportação de imagem do modelo.


**Repositório criado para fins educacionais e para auxiliar outros estudantes e profissionais da área de dados.**  
