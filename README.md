# Aurora Portal Claude Code Plugins

A collection of Claude Code plugins tailored for Aurora Portal development (PHP/Laravel + Vue.js).

## Plugins

### aurora-code-review

A comprehensive code review agent that analyzes PHP/Laravel and Vue.js code following Aurora Portal standards and best practices.

**Features:**

- Validates naming conventions (Portuguese for backend, English for frontend variables/methods)
- Checks folder structure compliance for Controllers, Services, DTOs, Validators, etc.
- Enforces REST patterns for routes and actions
- Reviews component organization in Vue.js
- Validates button colors and naming conventions
- Checks commit message format (Conventional Commits)
- Provides severity-based feedback (Critical, Warning, Suggestion)
- Generates summary with overall assessment

**Standards Covered:**

- PSR standards (PSR-1, PSR-4, PSR-12)
- Aurora Portal folder structure
- Controller/Service separation of concerns
- DTO patterns and transformers
- Vue.js component organization
- Route naming conventions
- Button styling standards
- Testing best practices

## Installation

Add the marketplace and install the plugin:

```
/plugin marketplace add aurora-portal/claude-code
```

Install the code review plugin:
```
/plugin install aurora-code-review@aurora-portal
```

## Usage

### Code Review

After making changes or before committing, ask Claude Code to review:

```
> Review my recent changes using the aurora-code-review agent
```

Or review specific files:

```
> Use aurora-code-review to analyze src/Modules/Compras/Controller/PedidosController.php
```

## Documentation

The code review rules are based on the Aurora Portal documentation found in the `docs/` folder, including:

- [Padroes](docs/padroes.md) - Coding standards and conventions
- [Componentes](docs/componentes.md) - Vue.js component guidelines
- [Services PHP](docs/servicesphp.md) - Service layer patterns
- [DTOs](docs/dto.md) - Data Transfer Objects guidelines
- [Validacao](docs/validacao.md) - Validation patterns
- [Testes](docs/testes.md) - Testing standards
