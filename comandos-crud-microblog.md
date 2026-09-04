# INSERT: Inserindo dados

```sql
INSERT INTO categorias (nome) VALUES('Tecnologia');
INSERT INTO categorias (nome) VALUES('Educação');
INSERT INTO categorias (nome) VALUES('Entreterimento');
```

```sql
INSERT INTO noticias (data, titulo, texto, imagem, resumo, destaque, usuario_id, categoria_id)
VALUES(
    04/09/2026
    'Barranco Desmorona',
    'Barranco se solta de ladeira lateral e se amontoa causando amontoado',
    'png',
    'Barranco Cai',
    80.99,
    100,
    4 -- id do fornecedor Livraria
);
```

