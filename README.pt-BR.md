# Análise de Dados de Vendas com Python
[English](README.md) | [Português](README.pt-BR.md)

## Visão Geral

Este projeto apresenta uma análise exploratória completa de um conjunto de dados sintético de vendas de e-commerce utilizando Python.

O objetivo é transformar dados transacionais em insights de negócio relacionados ao desempenho dos produtos, evolução do faturamento, distribuição geográfica e contribuição das categorias de produtos.

O projeto cobre todo o fluxo analítico, incluindo geração de dados sintéticos, exploração, limpeza, engenharia de atributos, agregações, visualização e interpretação dos resultados.

> **Observação:** Todos os dados utilizados neste projeto foram gerados sinteticamente em Python para fins educacionais e de portfólio. Eles não representam nenhuma empresa, cliente ou operação comercial real.

---

## Problema de Negócio

A operação de e-commerce está em crescimento e processa um volume cada vez maior de transações diárias. No entanto, dados brutos de vendas, por si só, não oferecem visibilidade suficiente para apoiar decisões de negócio de forma eficiente.

Os principais desafios abordados neste projeto são:

- baixa visibilidade sobre produtos de alto e baixo desempenho;
- entendimento limitado sobre a contribuição de cada categoria para o faturamento;
- ausência de uma visão estruturada da evolução mensal das vendas;
- baixa visibilidade geográfica para apoiar decisões de expansão e marketing.

---

## Perguntas de Negócio

A análise busca responder a quatro perguntas principais:

- **O que devemos vender?** Identificar os produtos de melhor desempenho e apoiar decisões de estoque e portfólio.
- **Onde devemos focar?** Entender quais categorias de produtos geram maior faturamento.
- **Quando devemos agir?** Analisar o desempenho mensal do faturamento e identificar variações relevantes ao longo do tempo.
- **Para onde devemos expandir?** Avaliar a distribuição do faturamento entre os estados brasileiros e identificar os mercados mais fortes.

---

## Dataset

O conjunto de dados contém **10.000 transações de vendas sintéticas**, geradas programaticamente em Python.

As principais informações disponíveis são:

- ID da venda;
- data da transação;
- produto;
- categoria do produto;
- preço unitário;
- quantidade vendida;
- ID do cliente;
- estado brasileiro;
- cidade.

O catálogo contém **50 produtos diferentes**, distribuídos entre categorias como:

- Electronics
- Hardware
- Furniture
- Accessories
- Networking
- Wearables
- Storage

Todos os valores monetários são expressos em **Real Brasileiro (BRL)**.

---

## Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Fluxo Analítico

1. Definição do problema de negócio
2. Importação das bibliotecas
3. Geração dos dados sintéticos
4. Carregamento e exploração inicial dos dados
5. Limpeza e pré-processamento
6. Engenharia de atributos
7. Análise de desempenho dos produtos
8. Análise do faturamento mensal
9. Análise geográfica do faturamento
10. Análise por categoria de produto
11. Interpretação dos resultados e conclusões

---

## Principais Insights

- **Network Switch** apresentou o maior volume de vendas, com **3.564 unidades vendidas**, seguido por Motherboard e Business Laptop.
- O faturamento mensal permaneceu relativamente estável ao longo do ano, variando entre aproximadamente **R$ 17,7 milhões e R$ 20,8 milhões**.
- **Outubro** apresentou o maior faturamento mensal, enquanto **junho** registrou o menor resultado.
- **Bahia e São Paulo** apresentaram os maiores faturamentos, ambos próximos de **R$ 24,9 milhões**.
- **Electronics** foi a categoria com maior geração de receita, alcançando aproximadamente **R$ 120,1 milhões**, significativamente acima das demais categorias.

Como o conjunto de dados é sintético e gerado aleatoriamente, esses resultados devem ser interpretados como saídas analíticas de um cenário simulado e não como comportamento real de mercado.

---

## Visualizações

### Top 10 Produtos Mais Vendidos

O ranking apresenta os produtos com maior volume de vendas no conjunto de dados sintético. Network Switch apresentou o maior volume, seguido de perto por Motherboard e Business Laptop.

![Top 10 Produtos Mais Vendidos](images/top10_products_quantity_sold.png)

### Faturamento Mensal

O faturamento mensal permaneceu relativamente estável ao longo do ano, variando entre aproximadamente R$ 17,7 milhões e R$ 20,8 milhões. Outubro apresentou o maior faturamento, enquanto junho registrou o menor resultado.

![Faturamento Mensal](images/monthly_revenue.png)

### Faturamento por Estado

O faturamento apresentou distribuição relativamente equilibrada entre os estados brasileiros analisados. Bahia e São Paulo registraram os maiores resultados, ambos próximos de R$ 24,9 milhões.

![Faturamento por Estado](images/revenue_by_state.png)

### Faturamento por Categoria de Produto

A categoria Electronics apresentou a maior contribuição para o faturamento, alcançando aproximadamente R$ 120,1 milhões. Hardware e Furniture ocuparam a segunda e terceira posições, respectivamente.

![Faturamento por Categoria](images/revenue_by_category.png)

---

## Estrutura do Projeto

```text
sales_data_analysis_ecommerce/
│
├── images/
│   ├── top10_products_quantity_sold.png
│   ├── monthly_revenue.png
│   ├── revenue_by_state.png
│   └── revenue_by_category.png
│
├── notebooks/
│   └── sales_analysis.ipynb
│
├── .gitignore
├── README.md
├── README.pt-BR.md
└── requirements.txt

```

---

## Como Executar

Clone o repositório:

```bash
git clone https://github.com/Guid3Paula/sales_data_analysis_ecommerce.git
```

Acesse a pasta do projeto:

```bash
cd sales_data_analysis_ecommerce
```

Crie um ambiente virtual:

```bash
python -m venv .venv
```

Ative o ambiente no Windows:

```bash
.venv\Scripts\Activate.ps1
```

Instale as bibliotecas necessárias:

```bash
python -m pip install -r requirements.txt
```

Abra o notebook:

```text
notebooks/sales_analysis.ipynb
```

Depois selecione o ambiente virtual do projeto como kernel do Jupyter.

---

## Próximas Evoluções

Possíveis evoluções futuras incluem:

- segmentação de clientes;
- análise de rentabilidade;
- análise de comportamento de compra;
- previsão de vendas;
- dashboards interativos;
- inclusão de novos KPIs comerciais.

---

## Conclusão

Este projeto demonstra como dados transacionais podem ser transformados em informações relevantes para o negócio por meio de um fluxo analítico completo utilizando Python.

Embora o conjunto de dados seja totalmente sintético, o projeto representa um cenário de negócio realista e demonstra como a análise de dados pode apoiar decisões relacionadas à gestão de estoque, planejamento comercial, priorização geográfica e portfólio de produtos.

O fluxo desenvolvido inclui geração de dados, exploração, limpeza, engenharia de atributos, agregações, visualizações e interpretação dos resultados.

---

## Aviso

Este projeto foi desenvolvido para fins educacionais e de portfólio.

O conjunto de dados é inteiramente sintético e não contém informações reais de clientes, empresas ou operações comerciais.