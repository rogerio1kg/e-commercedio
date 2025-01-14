# E-Commerce Entity-Relationship Diagram (EER)

Este repositório contém um diagrama de relacionamento entre entidades (EER) para um sistema de e-commerce, representando os principais componentes do sistema e suas relações. O diagrama foi refinado para incluir as seguintes funcionalidades:

- **Clientes PJ e PF**: Gerenciamento de contas separadas para pessoas físicas (PF) e jurídicas (PJ), garantindo que um cliente não possua ambas as informações simultaneamente.
- **Pagamento**: Suporte a múltiplas formas de pagamento cadastradas por pedido.
- **Entrega**: Adição de status e código de rastreio para o acompanhamento do envio dos pedidos.

## Estrutura do Diagrama

O diagrama EER é organizado em tabelas inter-relacionadas, descritas abaixo:

### Tabelas Principais

1. **Conta**
   - Armazena informações comuns de clientes, como nome e endereço.

2. **Cliente_PF**
   - Dados específicos para pessoas físicas, incluindo CPF e data de nascimento.

3. **Cliente_PJ**
   - Dados específicos para pessoas jurídicas, como CNPJ e razão social.

4. **FormaPagamento**
   - Lista as formas de pagamento disponíveis.

5. **Pedido**
   - Contém informações sobre pedidos, como status, descrição e frete.

6. **Entrega**
   - Inclui detalhes de envio, como status e código de rastreio.

7. **Produto**
   - Descreve os produtos disponíveis no sistema.

8. **Fornecedor**
   - Armazena dados dos fornecedores.

### Relacionamentos

- Cada cliente está associado a uma conta.
- Um pedido pode ter múltiplas formas de pagamento.
- Cada pedido está associado a uma entrega.
- Produtos são gerenciados em estoque e podem ser fornecidos por fornecedores específicos.

## Diagrama EER

![EER Diagram](https://github.com/rogerio1kg/e-commercedio/blob/main/modelo_EER-ecommerce.png)

O diagrama acima apresenta todas as tabelas e suas relações. Ele foi projetado para garantir um fluxo lógico de dados e facilitar a expansão do sistema, caso necessário.

## Como Usar Este Repositório

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```

2. Abra o arquivo do diagrama (`modelo_EER-ecomerce.png`) para visualizar a estrutura do banco de dados.

3. Use o modelo como referência para a implementação do banco de dados em sua aplicação.

## Contribuição

Contribuições são bem-vindas! Se você identificar melhorias ou ajustes no modelo, fique à vontade para abrir uma issue ou enviar um pull request.

## Licença

Este projeto está licenciado sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.
