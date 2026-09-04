# Comandos CRUD para o banco de dados Fly By Night

```sql
-- INSERT de fornecedores
INSERT INTO fornecedores (nome) VALUES('Eletrônicos Tabajara');
INSERT INTO fornecedores (nome) VALUES('Games ABCD'), ('Supermercado Tem de Tudo'),
('Livraria Demais da Conta');
```

## INSERT na tabela de Produtos

```sql
INSERT INTO produtos (nome, descricao, preco, quantidade, fornecedor_id)
VALUES(
    'Smartphone Galaxy S23',
    'Equipamento com Android e câmera Full HD e etc e tal',
    1599.45,
    20,
    1 -- id do fornecedor Eletrônicos Tabajara
);
```

```sql
INSERT INTO produtos (nome, descricao, preco, quantidade, fornecedor_id)
VALUES(
    'Senhor dos Anéis: As Duas Torres',
    'Volume 2 da série de livros criados pelo autor J.R.R Tolkien',
    80.99,
    100,
    4 -- id do fornecedor Livraria
);
```

```sql
INSERT INTO produtos (nome, descricao, preco, quantidade, fornecedor_id)
VALUES(
    'TV Led',
    'Tela de 50 polegadas, resolução 4K, 4 entradas HDMI e etc e tal',
    3420,
    12,
    1 -- id do fornecedor Eletônicos Tabajara
);
```

## INSERT na tabela Lojas

```sql
-- Insira as lojas: Casas Bahia, Shopping Zona Leste, Bazar e Americanas
```

```sql
INSERT INTO lojas (nome)
VALUES('Casas Bahia');
INSERT INTO lojas (nome)
VALUES('Shopping Zona Leste');
INSERT INTO lojas (nome)
VALUES('Bazar das Coisas');
INSERT INTO lojas (nome)
VALUES('Americanas');
```

## INSERT na tabela Lojas-Produtos

Esta é uma tabela intermediária (também conhecida como **tabela pivot**), ou seja, ela se relaciona com outras duas tabelas: **produtos** e **lojas** através de chaves estrangeiras.

```sql
INSERT INTO lojas_produtos(loja_id, produto_id, estoque) VALUES(2, 1, 20);

-- Insira também:
-- Senhor dos Anéis na loja Americanas, com estoque 3
-- TV Led no Shopping Zona Leste, com estoque 10
-- Smartphone nas Casas Bahia, com estoque 5
-- Smartphone na Americanas, com estoque 2
```

```sql
INSERT INTO lojas_produtos(loja_id, produto_id, estoque) VALUES(4, 2, 3);
```

```sql
INSERT INTO lojas_produtos(loja_id, produto_id, estoque) VALUES(2, 3, 10);
```

```sql
INSERT INTO lojas_produtos(loja_id, produto_id, estoque) VALUES(1, 1, 5);
```

```sql
INSERT INTO lojas_produtos(loja_id, produto_id, estoque) VALUES(4, 1, 2);
```