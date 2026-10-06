MER - Geek Store (Júnior)

1- Entidades

    Cliente: Quem compra na loja.

    Produto: Os itens colecionáveis (figures, games, etc.).

    Pedido: As compras realizadas.

2- Atributos

    Cliente:

        id_cliente (PK - Primary Key)

        nome

        email

        telefone

    Produto:

        id_produto (PK - Primary Key)

        nome

        categoria (Ex: "Figures", "Funkos", "Props")

        preco

        estoque

    Pedido:

        id_pedido (PK - Primary Key)

        data_pedido

        valor_total

        status (Ex: "Processando", "Enviado", "Entregue")

        id_cliente (FK - Foreign Key)

        id_produto (FK - Foreign Key)

3- Relacionamentos

    Cliente -> Pedido: 1 Cliente faz 1 ou vários Pedidos (1:N).

    Pedido -> Produto: 1 Pedido contém 1 ou vários Produtos (1:N).