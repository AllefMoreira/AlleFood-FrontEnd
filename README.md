# All-Food-FrontEnd

Esse é o front-end do desafio final do curso Explorer da RocketSeat. 🚀

## Tecnologias usadas :
O site foi contruido com **ReactJS**, e utilizando as seguintes Funcionalidades: 
- Styled Components; 
- React Icons; 
- React Router Dom; 
- Swiper.

## Usuários 
Neste projeto nós temos dois tipos de usuários, o admin e o cliente.

### admin 
O admin tem a tarefa de cuidar do site, adicionando, alterando e excluindo pratos, bebidas ou sobremesas. 

### cliente 
O cliente pode adicionar pratos aos favoritos, adicionar à lista de compras e poderia fazer a compras, mas eu optei por não fazer qualquer tratamento de dados sensíveis nesse projeto. 

## Funcionalidades: 

### Responsividade:
- O site é completamente responsivo, e um usuário no celular pode executar as mesmas funções de um usuário no computador, menos a pesquisa de prato pelo header.
- Quando em um celular, o header muda, adicionando o menu, onde podem ser encontrados os menus para sair, acessar os favoritos e, em caso de admin, adicionar novos pratos.

### Criação do usuário:
- Não existem validações para e-mail, além de não permitir duplicidades, porém a senha é obrigatório ter no mínimo 6 dígitos.
- Após isso, é só entrar normalemnte, onde é validado o email e a senha do usuário e é retornado o token de validação.
- Não é possível criar usuários administradores, todos já vêm como clientes por padrão, existindo somente um usuário admin.

### Edição:
- Pode ser acessado através do ícone de lápis que fica no topo do card de cada item.
- Qualquer campo pode ser alterado.
- Todos eles são obrigatórios, pois todos são de extrema importância para o funcionamento do site.

### Criação:
- Pode ser acessado atraves do botão "Novo Prato" no header, ou, em caso de uso mobile, pode ser acessado no menu do header. 
- Todos os campos devem ser preenchidos, incluindo descrições e ingredientes.
- O campo "Preço" não possui validação de quantidade de casas decimais, mas ao ser armazenado no banco, ele é armazenado com limite de 2 casas decimais.

### Pesquisa de pratos:
- Pode ser usando tanto o nome do prato, quanto o ingrediente.<br/>
- O ingrediente não é mostrado na página home, mas ao incluir ou clicar na imagem é possível acessar todos os dados do prato, incluindo seus ingredientes.

### Sistema de compras:

#### Inclusão de prato ao sistema de compras:
- O prato pode ser acessado clicando no botão de incluir, ou na imagem do prato.
- A quantidade só pode ser controlada pelos botões de + ou -, e é enviada ao incluir o prato.
- Ao clicar em incluir no card do prato, o cliente é encaminhado para a página principal do prato, onde é possível ver as informações e confirmar o pedido.
- Após confirmar, o prato fica na lista de pedidos, onde pode ser excluido ou finalizar a compra.

#### Carrinho de compras:
- No carrinho fica todos os pratos que foram adicionados pelo usuário, com nome, imagem, preço unitário e quantidade.
- O valor total é calculado a partir da soma da multiplicação entre preço unitário e quantidade de cada prato.
- A imagem de QR Code não leva a qualquer lugar de pagamento, e o botão que finalizaria a compra não tem tratamento de dados nenhum, é meramente ilustrativo.

### Sistema de favoritos:
- O usuário pode adicionar um prato aos favoritos clicando no ícone de coração que fica no topo do card.
- Ao clicar, o ícone muda sua forma pra sinalizar q está favoritado e também pode ser encotnrado em "meus favoritos" no header do site.
- O prato que está favoritado ficará na lista de favoritos, e ao clicar na imagem do prato ele é encaminhado para a página principal do prato com a quantidade 1.
- O prato pode ser excluído dos favoritos utilizando o botão que fica em baixo do nome do prato, na lista dos favoritos, ou clicando novamente no coração.
  
## Deploy
O site pode ser encontrado no link: https://allefood.netlify.app/
Para usufruir do "modo cliente" você pode criar um usuário normalmente ou usar um login padrão:
**usuário**: joao@gmail.com
**senha**: 123456

O front-end está hospedado no Netlify e o back-end está hospedado no Heroku.
