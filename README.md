# Portfólio Backend .NET | Mateus Silva

Bem-vindo ao meu ecossistema de desenvolvimento. Sou um desenvolvedor com mais de 5 anos de trajetória técnica sólida. Minha base foi construída no suporte avançado de sistemas ERP, onde atuei como o elo vital entre o cliente final e a engenharia. Hoje, migro essa maturidade para a construção de APIs robustas e escaláveis no ecossistema .NET.
-
## O Diferencial da Minha Experiência
Diferente de um desenvolvedor iniciante comum, trago comigo a vivência real de quem já resolveu problemas críticos em produção:

Consultas e Variações de Banco de Dados: Domínio em manipular e extrair dados em ambientes críticos usando SQL Server, PostgreSQL, MySQL e Firebird.

Ciclo de Feedback & Qualidade: Experiência em traduzir dores reais de clientes para especificações técnicas, testar correções em nível de banco e código, e validar a entrega final antes do deploy.

Maturidade de Negócio: Profundo entendimento de regras de negócio complexas de ERPs, garantindo que cada linha de código escrita tenha propósito comercial e impacto positivo no usuário final.
## Stack Técnica
Linguagens & Frameworks: C#, .NET 8/9/10, ASP.NET Core.

Arquitetura & Padrões: Clean Architecture, DDD (Domain-Driven Design), SOLID, Design Patterns.

Persistência: Entity Framework Core, Dapper, SQL Server, PostgreSQL, MySQL, Firebird.

Segurança & Qualidade: JWT, Identity, Fluent Validation, Docker.

# Projetos em destaque

### [IveComeToBook](https://github.com/m4tc0des/IveComeToBook) (Em Desenvolvimento)
Sistema Avançado de Gestão de Venda e Aluguel de Livros

Este projeto é meu principal laboratório de engenharia, onde aplico padrões de escala industrial para criar uma API desacoplada, segura e internacionalizada.
 ## Arquitetura e Princípios SOLID (Clean Architecture)
O projeto é estruturado seguindo os princípios do Domain-Driven Design (DDD) e da Clean Architecture, garantindo que a complexidade de negócio seja o coração da aplicação:

Camada de Domínio (Domain): O núcleo da aplicação, contendo as Entidades de Negócio puras e as Classes Base (EntityBase) para padronização de auditoria e identificação.

Camada de Aplicação (Application): Orquestração e serviços desacoplados via Extension Methods, mantendo o Program.cs limpo e modular.

Shared (Camadas Transversais):

Communication: Camada dedicada aos contratos da API, contendo Requests (ex: RequestRegisterUserJson) e Responses, protegendo o cliente externo de mudanças internas.

Exceptions & i18n: Centralização da lógica de erros com suporte nativo a múltiplos idiomas (Português, Inglês, Espanhol e Francês) via arquivos de recurso (.resx).

Infrastructure (Implementação SOLID):

I - Interface Segregation: Repositórios específicos que evitam dependências desnecessárias.

D - Dependency Inversion & Multi-DB: Interfaces intermediárias que permitem a comunicação transparente com SQL Server, PostgreSQL e MySQL, permitindo trocas de infraestrutura sem impacto no core.

Camada de API: Gerenciamento HTTP com Filtros Globais de Exceção, garantindo segurança e padronização total das respostas.

## Decisões de Engenharia
Mapster vs AutoMapper: Escolha estratégica pelo Mapster visando performance superior e conformidade de licenciamento (MIT).

Segurança de Dados: Mapeamentos customizados que ignoram campos sensíveis como Password, forçando o tratamento manual e seguro de credenciais.

Qualidade & Validação: Uso de Fluent Validation e ExceptionFilter para proteger detalhes internos (StackTrace) e fornecer retornos amigáveis ao front-end.

## Por que essa estrutura importa?
Essa organização reflete minha maturidade de mais de 5 anos no suporte técnico avançado. Nas empresas por onde passei, observei que solicitações simples de correção ou novas funcionalidades levavam semanas para serem integradas. Isso ocorria porque os projetos eram mal organizados: qualquer alteração exigia mexer em toda a estrutura, gerando um ciclo de instabilidade e retrabalho.

No IveComeToBook, aplico o oposto dessa realidade. Com responsabilidades claras (como manda o SRP do SOLID), a manutenção e os testes tornam-se tarefas ágeis. Um projeto bem estruturado não é apenas um "capricho técnico", mas uma necessidade para garantir a saúde do negócio e a velocidade da entrega.

