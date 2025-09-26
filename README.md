# Data Product Case Study – Análise de Retenção e Valor de Clientes

Este projeto simula a construção de um **data product** para analisar métricas de retenção (Churn) e valor de clientes (LTV – Lifetime Value) a partir de dados de e-commerce.  
O objetivo é **apoiar decisões de negócio** sobre quais mercados priorizar em termos de investimento, retenção e expansão.

- **Diagnosticar retenção de clientes**: medir churn rate por país.  
- **Avaliar valor dos clientes**: calcular LTV médio.  
- **Segmentar mercados**: identificar países de alto vs baixo potencial.  
- **Construir uma visão de cohorts**: entender comportamento de retenção ao longo do tempo.  


- **Fonte**: Online Retail dataset (UCI ML Repository).  
- **Fact Table**: `fact_orders` (transações individuais).  
- **Dim Tables**:  
  - `dim_customers`: informações derivadas de clientes (LTV, churn flag, país).  
  - `dim_products`: informações de produtos.  

- **LTV (Lifetime Value)** = total gasto por cliente ao longo do tempo.  
- **Churn rate** = % de clientes que não realizaram compras nos últimos 180 dias.  
- **Cohorts de retenção** = grupos de clientes por mês de aquisição, acompanhados ao longo do tempo.  

## Conclusões

### Mercados com maior churn (clientes perdidos)
- Brasil, Bahrein, Lituânia, Líbano → churn de 100% (clientes não retornaram).  
- Grécia, Canadá, EAU → churn ~50%.  

### Mercados com menor churn e maior valor
- Irlanda → LTV médio de ~90k €, churn = 0%.  
- Singapura → LTV médio de ~20k €, churn = 0%.  
- Islândia, Israel, Dinamarca → churn = 0%, mas LTV relativamente baixo.  

### Insights
- **Irlanda e Singapura são os mercados prioritários** → alta receita e clientes fiéis.  
- **Brasil e Bahrein devem ser despriorizados** → clientes não voltam após a primeira compra.  
- **Mercados de baixo LTV mas churn baixo (ex. Polónia, Malta)** → clientes leais, mas de baixo valor → oportunidade para upsell.  


