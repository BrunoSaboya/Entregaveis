
|Functions   |      Explicação      |
|----------|:--------------------:|
| _createNFT() |interna, checa se o número atual de tokens não atingiu o limite máximo e cria um novo token|
| ownerMint() | Função que apenas pode ser chamada pelo dono, chama _createNFT() |
| publicMint() | Função que pode ser chamada por todos, checa se o valor mandado ao contrato é maior que o preço para mintar um NFT, e se a venda esta aberta, chama _createNFT() |
| getTotalSupply() | devolve a quantidade de tokens já feita |
| setMintPrice() | Troca o preço do token a ser criado |
| openSales() | Possibilita a venda de tokens (mint), chama setMintPrice() com o novo preço|
| closeSales() | Impossibilita a venda de tokens (mint) |