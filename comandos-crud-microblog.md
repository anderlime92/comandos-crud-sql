# INSERT: Inserindo dados

```sql
INSERT INTO categorias (nome) VALUES('Tecnologia');
INSERT INTO categorias (nome) VALUES('Educação');
INSERT INTO categorias (nome) VALUES('Entreterimento');
```

```sql
INSERT INTO noticias (titulo, texto, imagem, resumo, destaque, usuario_id, categoria_id)
VALUES(
    'Barranco Desmorona',
    'Barranco se solta de ladeira lateral e se amontoa causando amontoado obstrutor',
    'barranco.png',
    'Barranco Cai e obstrui',
    'sim',
    3,
    2 
),
(
    'IA Térmica',
    'Estudantes da federal do sudoeste de Nárnia obtem avanços significativos com ajuda de nova IA térmica',
    'federal.png',
    'IA avança mecatrônica',
    'nao',
    2,
    1 
),
(
    'Full-Stack Revigorado',
    'Linguagem JEEP é a nova sensação que esta abalando o TI contenporâneo',
    'JEEP.png',
    'Linguagem JEEP revoluciona',
    'nao',
    1,
    1 
),
(
    'O Abismo Acorda',
    'Uma cabana misteriosa recebe a visitação de quatro agentes governamentais, nem eles e a platéia imaginavam o tamanho da treta',
    'saladecinema.png',
    'Nova estréia da semana',
    'nao',
    3,
    3 
);
```

```sql
INSERT INTO usuarios (nome, email, senha, tipo)
VALUES(
    'Ana Silva',
    'ana@email.com',
    '123abc',
    'editor'
),
(
    'Bruno Souza',
    'bruno@email.com',
    'abc456',
    'admin'
),
(
    'Carla Mendes',
    'carla@email.com',
    '789xyz',
    'editor'
);
```

```sql
-- Correção abaixo
```

```sql
INSERT INTO usuarios(nome, email, senha, tipo) 
VALUES('Ana Silva', 'ana@email.com', '123abc', 'editor'),
VALUES('Bruno Souza', 'bruno@email.com', 'abc456', 'admin'),
VALUES('Carla Mendes', 'carla@email.com', '789xyz', 'editor');
```
## INSERT na tabela categorias

```sql
INSERT INTO noticias(titulo, texto, imagem, destaque, usuario_id, categoria_id)
VALUES(
    'Corinthians está mau pra caramba',
    'O time caiu muito após a copa do mundo',
    'Não sei mais o que escrever sobre isso tudo e etc e tal e bla bla',
    'corinthians',
    'nao',
    3,
    3
);
```
```sql
INSERT INTO noticias(titulo, texto, imagem, destaque, usuario_id, categoria_id)
VALUES(
    ''
    ''
    ''
    ''
), (
    ''
    
)

## INSERT na tabela noticias