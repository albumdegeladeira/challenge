# Desafio Fullstack Node.js Da Album de Geladeira

Esse desafio tem como objetivo testar as competências de desenvolvimento frontend (React) e backend (node.js).

Deverá ser construída uma aplicação concisa que simula o funcionamento de uma das partes mais importantes de um e-commerce. O carrinho.

### Frontend
O frontend da aplicação deve possuir duas rotas: 
- /produtos 
    - mostra uma listagem simples dos produtos disponiveis
    - os produtos devem ser obtidos através de uma rota no backend
    - dá opção de adicionar ao carrinho em cada item
- /carrinho 
    - Exibe os itens atualmente no carrinho ou uma tela com mensagem de "carrinho vazio!". 
    - Devem ser exibidas as quantidades de cada item e o usuário deve conseguir adicionar e remover itens alterando a quantidade. 
    - Itens que chegarem a quantidade 0 devem ser removidos da lista.
    - Um subtotal deve ser exibido, mostrando o somatório de de todos os produtos sem o valor do frete
    - Um campo para calculo do frete deve ser exibido em conjunto com um botão que faz a solicitação para o backend que retorna o prazo de entrega em dias e o custo do frete
    - Um total deve ser exibido, mostrando o somatório de todos os produtos no carrinho + valor do frete
- informações adicionais: 
    - O estado do carrinho deve ficar salvo entre páginas e até mesmo se o usuário sair da página e voltar.

    O frontend deve ser construído em React em conjunto com qualquer biblioteca do ecosistema que o candido julgar necessária a inclusão.
    Uso de create-react-app é recomendado porém não obrigatório.

Bônus se usar: styled-components, typescript



### Backend
O backend deve ser uma api simples que consiste em duas rotas:

- /products provê a lista de produtos disponíveis para serem exibidos em /produtos no frontend. Os dados podem ser definidos estaticamente, sem necessidade de consumir de um banco de dados.
- /shipping:cep
    - recebe o cep e retorna o prazo de entrega em dias e o custo de envio para sedex (Pode fazer funcionar com apenas alguns valores fixos, mas usar a api dos correios seria um bônus interessante)
    - fatores como peso, tamanho e quantidade de produtos não devem ser considerados

Bônus se usar: express
