# Template para API's

Este repositório se destina a um modelo genérico que elaborei com base nos meus estudos e trabalhos durante minha carreira como programador Backend.

## Por quê?

- Estruturar um projeto é sempre uma tarefa chatinha, mas muito importante, então pensando nisso decidi de criar um modelo genérico para API's, para evitar ter que ficar pensando na estrutura todo projeto que começo.

- Novas ideias e necessidades irão surgir, permitindo que esse modelo seja atualizado e melhorando para atender as demandas de cada projeto (Mas ainda assim ajudará quem está começando)

## Estrutura do Projeto

O projeto está modularizado para poder separar e organizar todas as demandas do projeto e ajudar o desenvolvedor na hora de montar sua API.

Na raiz do nosso projeto, teremos algumas pastas e arquivos importantes para a API como:

- Arquivos
  - .env (Responsável por guardar as variáveis de ambiente que nossa API precisará)
  - README.md (Responsável por explicar o que é o projeto e como deve ser executado)
- Pastas
  - .vscode (Responsável por configurar padrões no `VS CODE` para aplicar em todos os usuários do projeto, como padrões de projeto, formatação de código, etc.)
    - settings.json (Guarda todas as configurações para aplicar no projeto)
  - docs (Responsável por guardar todos os arquivos de documentação da API, como diagramas, regras de negócio)
  - app (Todos os diretórios e Conteúdo que a API usará)
    - constants (Responsável por armazenar todos os arquivos de contantes que a aplicação precisará para operar, facilitando a manutenção)
    - controllers (Responsável por todas as manipulações de Ações no Banco de Dados, mediante regras de negócio)
    - core (Responsável por todas as dependências da regra de negócio, como contratos, cálculos financeiros, etc.)
    - database (Responsável por gerenciar as conexões com o banco de dados, além do mapeamento das tabelas e registros em objetos)
    - hooks (Responsável por disparar webhooks em caso de eventos específicos da aplicação)
    - images (Responsável por armazenar imagens que a aplicação do frontend consuma)
    - routes (Responsável por implementar os endpoints que a API estará fornecendo)
    - schemas (Responsável por mapear as estruturas de dados que estarão trafegando entre o backend e o frontend)
    - services (Responsável por serviços genéricos envolvendo autenticação ou acesso à API de terceiros como gateways de pagamento, etc.)
    - tests (Responsável por validar se toda a API está funcionando como deveria)
    - utils (para armazenar funções utilitárias e helpers reutilizáveis em diferentes partes do projeto. Como conversões de dados, injetar dependências, logs e validações)

### Visualização

```plaintext
api/
├── .vscode/
│   ├── settings.json
├── docs/
│   ├── funcionalidades.md
│   ├── regras_de_negocio.md
│   └── manual_usuario.md
├── app/
│   ├── constants/
│   ├── controllers/
│   ├── core/
│   ├── database/
│   ├── hooks/
│   ├── images/
│   ├── routs/
│   ├── schemas/
│   ├── services/
│   ├── tests/
│   ├── utils/

├── .env
├── README.md 
```
