R.F. 01 - Registro de usuário no sistema: permite que novos usuários se cadastrem para acessar o site e realizar compras.
Dados necessários: nome, e-mail, senha, endereço.

Usuários: visitantes.

R.F. 02 - Registro de produto pelo administrador: permite o cadastro de novos produtos naturais no sistema.
Dados necessários: nome do produto, categoria, preço, imagem, descrição, quantidade em estoque.

Usuários: administrador.

Tipo: Funções Administrativas / Gestão de Dados.

R.F. 03 - Inserção de item no carrinho de compras: permite ao usuário adicionar produtos selecionados ao carrinho.
Dados necessários: produto, quantidade, ID do usuário (sessão).

Usuários: cliente autenticado.

Tipo: Gestão de Dados / Regulamentos de Negócio.

🔄 Processamentos
R.F. 04 - Autenticação de usuário: autentica o acesso do usuário ao sistema, garantindo segurança e acesso à sua conta.
Dados necessários: e-mail, senha.

Usuários: todos os níveis de usuário.

Tipo: Níveis de autorização.

R.F. 05 - Processamento de pedido (checkout): processa as informações do carrinho, endereço e pagamento para gerar o pedido.
Dados necessários: produtos, endereço, forma de pagamento, cupom (opcional).

Usuários: cliente autenticado.

Tipo: Gestão de Dados / Interfaces Externas (pagamento).

R.F. 06 - Aplicação de cupom de desconto: valida e aplica o cupom inserido conforme as regras de negócio.
Dados necessários: código do cupom, valor do pedido, categoria dos produtos.

Usuários: cliente autenticado.

Tipo: Regulamentos de Negócio.

R.F. 07 - Atualização de status do pedido: atualiza o pedido com os status: “em processamento”, “enviado”, “entregue”.
Dados necessários: ID do pedido, status novo.

Usuários: administrador, cliente autenticado (apenas visualização).

Tipo: Regulamentos de Negócio / Rastreamento de auditoria.

R.F. 08 - Avaliação de produtos: permite que o usuário avalie e comente produtos adquiridos.
Dados necessários: nota, comentário, ID do produto, ID do pedido.

Usuários: cliente autenticado.

Tipo: Gestão de Dados.

📤 Saídas
R.F. 09 - Exibição de listagem de produtos: mostra ao cliente todos os produtos disponíveis para compra com filtros.
Dados necessários: nome do produto, imagem, preço, descrição curta, categoria.

Usuários: todos os usuários.

Tipo: Gestão de Dados / Interfaces Externas.

R.F. 10 - Exibição de detalhes de produto: mostra informações completas sobre o produto selecionado.
Dados necessários: nome, descrição, benefícios, ingredientes, forma de uso, avaliações.

Usuários: todos os usuários.

Tipo: Gestão de Dados.

R.F. 11 - Relatório de pedidos realizados: exibe histórico de pedidos do cliente.
Dados necessários: número do pedido, data, status, valor total, itens comprados.

Usuários: cliente autenticado.

Tipo: Requisitos de relatório.

R.F. 12 - Relatório de vendas por produto: exibe ao administrador dados sobre quantidade de vendas por item.
Dados necessários: nome do produto, total de vendas, receita gerada.

Usuários: administrador.

Tipo: Requisitos de relatório.
