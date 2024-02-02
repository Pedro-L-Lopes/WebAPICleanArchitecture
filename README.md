# API Catálogo - Clean Architecture

## Descrição
Esta é uma Web API desenvolvida em C# .NET 6 que gerencia um catálogo de produtos e categorias, utilizando um banco de dados SQL Server. A arquitetura utilizada é a Clean Architecture, proporcionando uma estrutura modular e de fácil manutenção.

## Pré-requisitos
- [.NET 6 SDK](https://dotnet.microsoft.com/download/dotnet/6.0)
- [SQL Server](https://www.microsoft.com/sql-server)

## Estrutura do Projeto
A estrutura do projeto segue os princípios da Clean Architecture, com divisão em camadas:

- Api: Contém os controladores e a configuração da API.
- Application: Responsável pela lógica de negócios da aplicação.
- Domain: Define as entidades e regras de negócio.
- Infrastructure: Implementa detalhes técnicos, como acesso a banco de dados e serviços externos.
- Catalogo.CrossCutting: Esta camada representa o conceito de Cross-Cutting Concerns, que são aspectos transversais à aplicação, como logging, validação, e outros. Aqui, você pode encontrar utilitários e serviços compartilhados entre as camadas, contribuindo para a coesão e reusabilidade do código.

# Vantagens da Clean Architecture
- Manutenibilidade: A estrutura modular facilita a manutenção e evolução do código.
- Testabilidade: A separação de responsabilidades torna mais fácil a criação de testes unitários e de integração.
- Independência de Frameworks: As camadas internas não dependem de frameworks externos, proporcionando flexibilidade para trocar ou atualizar tecnologias.

# Desvantagens da Clean Architecture
- Complexidade Inicial: Pode parecer complexa para projetos pequenos ou simples, adicionando um tempo inicial para a configuração e compreensão da estrutura, o que pode afetar a agilidade no desenvolvimento.
- Custo de Hospedagem: Pode haver um custo mais elevado para a hospedagem, dependendo da arquitetura escolhida e dos requisitos de recursos. Isso deve ser considerado, especialmente em ambientes onde os custos operacionais são críticos.
