# Webscrapping - Marketplace brasileiro (Roupas)

- [Webscrapping - Marketplace brasileiro (Roupas)](#webscrapping---marketplace-brasileiro-roupas)
  - [1. Disponibilização dos dados e códigos](#1-disponibilização-dos-dados-e-códigos)
    - [Datasets](#datasets)
    - [Códigos](#códigos)
  - [2. Informações do dataset](#2-informações-do-dataset)


O repositório apresenta a base de dados de mais de 2200 roupas, retirados do catálogo de um marketplace brasileiro por meio de webscrapping. Além do dataset, foram disponibilizados os códigos de scrapping e limpeza dos dados obtidos.
Por questões de segurança, o nome do marketplace não é mencionado nessa documentação ou nos códigos mas, no momento dessa redação, o site representa a maior plataforma de compra e vendas do Brasil.

## 1. Disponibilização dos dados e códigos

### Datasets
- [Base de dados limpa, com correção nos tipos de dados e colunas](dataset_roupas_marketplacebr_limpo.csv)
- [Base de dados crua, retirada diretamente do scrapping](scrapping_roupas_marketplace.csv)
- [Kaggle](https://www.kaggle.com/datasets/ulissescastro/brazil-clothing-marketplace-dataset)

### Códigos
- [Webscrapping para obtenção dos dados](webscrapper.ipynb)
- [Limpeza da base de dados obtida por scrapping](limpeza-dataset.ipynb)

## 2. Informações do dataset

O dataset limpo contém 2206 observações, separadas em 14 colunas. Os dados foram obtidos a partir da extração do site no dia 15/09/2023. As descrições das colunas estão disponíveis abaixo.

|   | **Coluna**               | **Descrição**                                                                                       | **Tipo**          |
|---|--------------------------|-----------------------------------------------------------------------------------------------------|-------------------|
|   | **Titulo**               | _Título do produto como apresentado no anúncio da venda_                                            | Categórica        |
|   | **Preco_original**       | _Preço original do item_                                                                            | Numérica contínua |
|   | **Desconto_percentual**  | _Percentual de desconto aplicado ao item_                                                           | Numérica contínua |
|   | **Preco_com_desconto**   | _Preço final do item com o desconto aplicado_                                                       | Numérica contínua |
|   | **n_vendidos_categoria** | _Categoria com o número de itens vendidos. O site categoriza o número de vendas a partir de ranges_ | Categórica        |
|   | **Marca**                | _Marca da roupa vendida_                                                                            | Categórica        |
|   | **Material**             | _Material da roupa_                                                                                 | Categórica        |
|   | **Gênero**               | _"Gênero" do item_                                                                                  | Categórica        |
|   | **Temporada**            | _Temporada do ano a qual a peça faz referência: Outono/Inverno, Primavera/Verão, etc._              | Categórica        |
|   | **Nota**                 | _Nota média das avaliações dos clientes_                                                            | Numérica contínua |
|   | **N_Avaliações**         | _Quantidade de avaliações dos clientes_                                                             | Numérica contínua |
|   | **Review1**              | _Primeira review que aparece na página do produto_                                                  | Categórica        |
|   | **Review2**              | _Segunda review que aparece na página do produto_                                                   | Categórica        |
|   | **Review3**              | _Terceira review que aparece na página do produto_                                                  | Categórica        |