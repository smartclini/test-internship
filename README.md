# Teste para vaga de estágio

## Desafio

**Objetivo**: Criar um pequeno sistema em Angular que permita listar e adicionar clientes usando um formulário. O sistema deve ser capaz de listar os clientes cadastrados e permitir a adição de novos clientes.

### Requisitos

1. Módulo de Clientes:
    - Criar um módulo chamado `ClientModule` para agrupar todos os componentes e serviços relacionados à funcionalidade de clientes.

2. Service para Manipulação de Dados:
    - Criar um serviço chamado `ClientService` que será responsável por armazenar e gerenciar os dados dos clientes.
    - O service deve incluir os métodos:
        - `addClient(client)`: Adicionar um novo cliente.
        - `getClients()` Retornar a lista de todos os clientes.
    - Os dados dos clientes serão armazenados em um array dentro do service.  Este array deve ser inicializado vazio e preenchido conforme novos clientes são adicionados.

3. Componente de Formulário:
    - Criar um componente chamado `ClientFormComponent` para gerenciar o formulário de adição de clientes.
    - O formulário deve incluir os seguintes campos:
        - `Nome`: Campo de texto obrigatório.
        - `E-mail`: Campo de texto obrigatório e deve ser validado para ser um e-mail válido.
        - `Telefone`: Campo de texto opcional, mas deve ser validado para conter apenas números.
    - O formulário deve ter um botão de submissão que, ao ser clicado, adiciona o cliente à lista de clientes no `ClientService`.

4. Componente para Listagem de Clientes:
    - Criar um componente chamado `ClientListComponent` para listar os clientes cadastrados.
    - O componente deve mostrar uma lista de clientes com as informações básicas (nome e e-mail).
    - Obter a lista de clientes diretamente do `ClientService`.
    - Nele deve ter um botão para adicionar um novo cliente, que deve abrir o formulário de adição de clientes.

### Estrutura de Arquivos Esperada:

- `src/app/features/client/client.module.ts`: Módulo do cliente.
- `src/app/features/client/components/client-form/client-form.component.ts`: Componente de formulário de cliente.
- `src/app/features/client/components/client-list/client-list.component.ts`: Componente de listagem de clientes.
- `src/app/features/client/services/client.service.ts`: Service para manipulação de dados de clientes.

### Sugestões para Avaliação:

- **Organização do Código**: Verificar se o código está bem estruturado, usando as convenções e boas práticas do Angular.

- **Validações**: Avaliar se o formulário inclui validações adequadas e fornece feedback claro ao usuário.

- **Funcionalidade**: Testar se a aplicação funciona conforme descrito, permitindo adicionar e listar clientes corretamente.

- **Uso de Bibliotecas de Estilo**: Você pode ficar à vontade para usar bibliotecas externas, como Bootstrap ou outras de sua preferência, para estilizar os componentes e melhorar a aparência do sistema.

### Entrega

- **Prazo**: 14 dias a partir do recebimento do teste.
- **Formato**: Crie um repositório público no GitHub para o seu projeto. Após subir o projeto, disponibilize o link para o repositório.