Descrição

O CP2 Application é uma aplicação web desenvolvida com ASP.NET Core 8.0, que utiliza Entity Framework Core 8.0 para interações com o banco de dados Oracle. A aplicação tem como objetivo gerenciar fornecedores e vendedores, permitindo operações como criar, editar, deletar e listar registros. Esta aplicação adota uma arquitetura baseada em camadas, que separa responsabilidades em diferentes módulos: Domain, Application, Data, API e IoC.
Estrutura do Projeto

O projeto é dividido nas seguintes camadas:
CP2.Domain: Contém as entidades e interfaces que representam as regras e conceitos do domínio da aplicação.
CP2.Application: Contém a lógica de negócios e as regras de validação. Esta camada implementa serviços que utilizam os repositórios.
CP2.Data: Responsável pela interação com o banco de dados utilizando o Entity Framework Core.
CP2.API: Fornece a API RESTful com endpoints para as operações CRUD de fornecedores e vendedores.
CP2.IoC: Configura a Injeção de Dependência (Dependency Injection) para serviços e repositórios, facilitando o gerenciamento de dependências no projeto.
Funcionalidades

Gerenciamento de Fornecedores:
Adicionar, editar, deletar e listar fornecedores.
Gerenciamento de Vendedores:
Adicionar, editar, deletar e listar vendedores.
Tecnologias Utilizadas

ASP.NET Core 8.0
Entity Framework Core 8.0 (suporte para Oracle)
Oracle Database para armazenamento de dados
Swagger para documentação automática da API
FluentValidation para validação dos DTOs
Instalação

Pré-requisitos
.NET 8.0 SDK ou superior
Banco de Dados Oracle configurado
Oracle Entity Framework Core Package instalado
Editor como Rider ou Visual Studio Code


Clone o repositório:
https://github.com/Nxtlevelbr/dotnetcp2
Execute as migrations para configurar o banco de dados:

dotnet ef database update
Inicie a aplicação:
dotnet run



