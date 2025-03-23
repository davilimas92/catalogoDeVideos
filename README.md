Microserviço: Admin do Catálogo de Vídeos
Este repositório contém o código-fonte de um microserviço que gerencia o Catálogo de Vídeos, com operações como adicionar, editar, remover e listar vídeos, além de gerenciar categorias e gêneros. Este microserviço foi desenvolvido utilizando as melhores práticas de mercado, como Clean Architecture, DDD, TDD e práticas modernas de desenvolvimento.

Arquitetura
Este microserviço segue a arquitetura Clean Architecture, que promove o desacoplamento entre os componentes, garantindo que a lógica de negócios seja isolada de implementações de frameworks, bancos de dados e interfaces de usuário.

A arquitetura é estruturada em camadas:

Entidades: Representa os objetos de domínio do catálogo de vídeos (ex.: Vídeo, Categoria, Gênero).
Use Cases: Contém a lógica de negócios principal (ex.: Adicionar vídeo, Editar vídeo, Listar vídeos).
Interfaces: Interfaces de comunicação com o banco de dados e outros sistemas (ex.: repositórios e APIs).
Frameworks e Drivers: Implementações específicas de frameworks e ferramentas externas (ex.: Spring Boot, RabbitMQ).
Tecnologias Utilizadas
Java 17: Linguagem principal do microserviço.
Spring Boot: Framework para criação de APIs RESTful.
RabbitMQ: Fila de mensagens utilizada para comunicação com o serviço de encoding de vídeos.
JPA (Hibernate): Implementação de persistência de dados.
JUnit 5 / Mockito: Ferramentas para testes unitários (TDD).
Maven: Gerenciador de dependências e construção do projeto.
Funcionalidades
Gerenciamento de Vídeos: Adicionar, editar, listar e excluir vídeos no catálogo.
Gerenciamento de Categorias e Gêneros: Criar e editar categorias e gêneros de vídeos.
Integração com Encoder de Vídeos: Envia vídeos para o serviço de encoding de vídeos via RabbitMQ.
API RESTful: Exposição de endpoints para interagir com o catálogo de vídeos.
