## Diagrama de Classes

- **Usuário**
  - ID: int
  - Nome: string
  - Email: string
  - Tipo: string
  - Registar()
  - FazerLogin()
  - AdicionarAoCarrinho(Produto produto)
  - Comprar()

- **Produto**
  - ID: int
  - Nome: string
  - Preço: float
  - Descrição: string
  - ExibirDetalhes()

- **Carrinho de Compras**
  - Itens: lista de Produto
  - Total: float
  - AdicionarItem(Produto produto)
  - RemoverItem(Produto produto)
  - CalcularTotal()
  - FinalizarCompra()

**Relações:**

- Um Usuário pode ter vários Produtos para venda (relação 1 para muitos entre Usuário e Produto).
- Um Usuário pode ter um Carrinho de Compras (relação 1 para 1 entre Usuário e Carrinho de Compras).
- Um Carrinho de Compras contém vários Produtos (relação muitos para muitos entre Carrinho de Compras e Produto).
