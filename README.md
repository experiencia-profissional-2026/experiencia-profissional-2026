# Experiência Profissional — Desenvolvimento de Aplicações | ESOFT

## 📘 Padrões, Regras e Boas Práticas

Este documento define os padrões e convenções adotados neste repositório do projeto para garantir organização, qualidade, colaboração eficiente e manutenção a longo prazo.

---

### 📌 1. Objetivo

Este projeto deve seguir boas práticas de desenvolvimento para:

* Facilitar a colaboração
* Reduzir erros
* Padronizar entregas
* Melhorar legibilidade
* Garantir escalabilidade

Todos os colaboradores devem seguir este guia.

---

### 📂 2. Estrutura de Pastas

Utilize uma organização clara e previsível, como por exemplo:

```
/
├── docs/           # Documentação
├── src/            # Código-fonte
├── tests/          # Testes automatizados
├── scripts/        # Scripts auxiliares
├── .github/        # Configurações do GitHub
├── README.md
└── .gitignore
```

Regras:

* Evite pastas genéricas como `temp/` ou `misc/`
* Cada módulo deve ter responsabilidade clara

---

### 🏷️ 3. Nomenclatura de Arquivos e Pastas

#### 📁 Pastas

Padrão:

```
kebab-case
```

Exemplo:

```
user-service
payment-module
```

#### 📄 Arquivos

Padrão geral:

```
kebab-case.ext
```

Exemplos:

```
user-controller.ts
order-service.js
config-loader.py
```

Exceções:

* Classes: `PascalCase.java`
* Componentes React: `PascalCase.jsx`

---

### 🧾 4. Padrões de Código

#### 📐 Convenções

| Elemento  | Padrão      | Exemplo           |
| --------- | ----------- | ----------------- |
| Variável  | camelCase   | `minhaVariavel`   |
| Função    | camelCase   | `calcularTotal()` |
| Classe    | PascalCase  | `MinhaClasse`     |
| Constante | UPPER_SNAKE | `VALOR_PI`        |
| Interface | PascalCase  | `UserRepository`  |

---

### 🌱 5. Padrão de Branches

Utilize o modelo:

```
<tipo>/<descricao-curta>
```

#### Tipos Permitidos

| Tipo     | Uso                 |
| -------- | ------------------- |
| feature  | Nova funcionalidade |
| fix      | Correção de bug     |
| hotfix   | Correção urgente    |
| refactor | Refatoração         |
| docs     | Documentação        |
| test     | Testes              |
| chore    | Manutenção          |

#### Exemplos

```
feature/login-social
fix/validacao-email
refactor/auth-service
docs/api-guide
```

---

### 📦 6. Commits

Utilizamos Conventional Commits.

Formato:

```
<tipo>(escopo): mensagem
```

#### Tipos

| Tipo     | Uso          |
| -------- | ------------ |
| feat     | Nova feature |
| fix      | Bug          |
| docs     | Documentação |
| style    | Formatação   |
| refactor | Refatoração  |
| test     | Testes       |
| chore    | Manutenção   |

#### Exemplos

```
feat(auth): adicionar login por token
fix(api): corrigir status 500
docs(readme): atualizar instruções
```

---

### 🔍 7. Pull Requests (PR)

#### 📋 Padrão de Título

```
[tipo] descrição curta
```

Exemplo:

```
[feat] Implementa autenticação JWT
[fix] Corrige cálculo de impostos
```

#### 📝 Template de PR

Todo PR deve conter:

* Descrição clara
* Motivação da mudança
* Evidências/testes
* Issues relacionadas

Modelo:

```md
## Descrição

## Motivação

## Como testar

## Issues relacionadas
```

---

### ✅ 8. Revisão de Código

Regras:

* Pelo menos 1 revisor
* Nenhum merge sem aprovação
* Código deve passar nos testes

Checklist:

* [ ] Código legível
* [ ] Testes adicionados
* [ ] Documentação atualizada
* [ ] Sem warnings

---

### 🧪 9. Testes

Requisitos:

* Todo código novo deve conter testes
* Cobertura mínima: 80% (decidiremos depois...)
* Testes devem ser automatizados

Padrão:

```
<arquivo>.spec.ts
<arquivo>.test.js
```

---

### 📖 10. Documentação

* README sempre atualizado
* APIs documentadas
* Use `docs/` para documentação extensa

---

### 🔐 11. Segurança

* Nunca commitar senhas
* Usar `.env`
* Adicionar `.env` ao `.gitignore`

---
