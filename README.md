# Aurora Portal - Plugins para Claude Code

Uma coleção de plugins do Claude Code desenvolvidos para o desenvolvimento do Aurora Portal (PHP/Symfony + Vue.js).

## Plugins

### aurora-code-review

Um agente abrangente de revisão de código que analisa código PHP/Symfony e Vue.js seguindo os padrões e boas práticas do Aurora Portal.

**Funcionalidades:**

- Valida convenções de nomenclatura (português para backend, inglês para variáveis/métodos do frontend)
- Verifica conformidade da estrutura de pastas para Controllers, Services, DTOs, Validators, etc.
- Aplica padrões REST para rotas e ações
- Revisa organização de componentes Vue.js
- Valida cores e nomenclatura de botões
- Verifica formato de mensagens de commit (Conventional Commits)
- Fornece feedback baseado em severidade (Crítico, Alerta, Sugestão)
- Gera resumo com avaliação geral

**Padrões Cobertos:**

- Padrões PSR (PSR-1, PSR-4, PSR-12)
- Estrutura de pastas do Aurora Portal
- Separação de responsabilidades Controller/Service
- Padrões de DTOs e transformers
- Organização de componentes Vue.js
- Convenções de nomenclatura de rotas
- Padrões de estilização de botões
- Boas práticas de testes

## Instalação

Adicione o marketplace e instale o plugin:

```
/plugin marketplace add aurora-portal/claude-code
```

Instale o plugin de revisão de código:
```
/plugin install aurora-code-review@aurora-portal
```

## Uso

### Revisão de Código

Após fazer alterações ou antes de commitar, peça ao Claude Code para revisar:

```
> Revise minhas alterações recentes usando o agente aurora-code-review
```

Ou revise arquivos específicos:

```
> Use aurora-code-review para analisar src/Modules/Compras/Controller/PedidosController.php
```

## Documentação

As regras de revisão de código são baseadas na documentação do Aurora Portal encontrada na pasta `docs/`, incluindo:

- [Padrões](docs/padroes.md) - Padrões e convenções de codificação
- [Componentes](docs/componentes.md) - Diretrizes de componentes Vue.js
- [Services PHP](docs/servicesphp.md) - Padrões da camada de serviços
- [DTOs](docs/dto.md) - Diretrizes de Data Transfer Objects
- [Validação](docs/validacao.md) - Padrões de validação
- [Testes](docs/testes.md) - Padrões de testes
