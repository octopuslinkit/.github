## 🐙 Octopus Link IT

**Octopus Link IT** é uma empresa de tecnologia focada no desenvolvimento de **soluções digitais próprias**.

Assim como um polvo, nossos tentáculos se estendem pela web — **conectando ideias, inovação e tecnologia**.  
Projetamos, desenvolvemos e evoluímos produtos com foco em **escalabilidade, qualidade e valor a longo prazo**.

Nosso trabalho é guiado por:

- Código limpo e de fácil manutenção
- Processos e padrões claros
- Colaboração e melhoria contínua
- Tecnologia a serviço de necessidades reais de negócio

---

## 📑 Sumário

- [Padrão de Branches e Commits](#-padrão-de-branches-e-commits)

---

# 📌 Padrão Oficial de Branches e Commits

Este documento define o padrão único e obrigatório de **branches** e **commits** do projeto.

O padrão é baseado na especificação **Conventional Commits**:  
https://www.conventionalcommits.org/pt-br/v1.0.0-beta.4/#especifica%C3%A7%C3%A3o

Objetivos:
- Histórico de commits claro e padronizado
- Rastreabilidade direta com issues
- Suporte a automações (changelog, versionamento, CI/CD)
- Facilidade de revisão de código

---

## 🌿 1. Padrão de Branches

### 📐 Formato Obrigatório

`<tipo>/<numero-da-issue>-<descricao-curta>`

### ✅ Regras Gerais
- Criar branches a partir de `develop`
- Usar apenas letras minúsculas
- Separar palavras com `-`
- O número da issue é **obrigatório**
- A descrição deve ser curta e objetiva
- Não usar caracteres especiais

---

### 🧩 Tipos de Branch Permitidos

| Tipo        | Quando usar |
|------------|------------|
| `feat`     | Nova funcionalidade |
| `fix`      | Correção de bug |
| `docs`     | Alterações apenas em documentação |
| `style`    | Ajustes visuais, lint, formatação |
| `refactor` | Refatoração sem mudança de comportamento |
| `test`     | Criação ou ajuste de testes |
| `chore`    | Manutenção do projeto |
| `perf`     | Melhorias de performance |
| `ci`       | Alterações em CI/CD |

---

### 📌 Exemplos de Branch

`feat/15-add-login-form`
`fix/42-fix-password-validation`
`refactor/18-clean-auth-service`
`chore/30-update-eslint-config`
`docs/12-update-readme`

---

## 📝 2. Padrão de Commits

### 📐 Formato Obrigatório

`<tipo>[escopo opcional]: <descricao> (#<numero-da-issue>)`

### 📌 Exemplo

`feat(auth): add login form (#15)`

---

### ✅ Regras Gerais
- O commit **DEVE** começar com um tipo válido
- A descrição **DEVE** usar verbo no imperativo
- O número da issue **É OBRIGATÓRIO**
- O escopo é opcional, mas recomendado
- Não usar ponto final no final da descrição
- A primeira linha não deve ultrapassar 100 caracteres

---

### 🧩 Tipos de Commit Permitidos

| Tipo        | Descrição |
|------------|-----------|
| `feat`     | Nova funcionalidade |
| `fix`      | Correção de bug |
| `docs`     | Mudanças na documentação |
| `style`    | Formatação, lint, espaços (sem lógica) |
| `refactor` | Refatoração sem alterar comportamento |
| `test`     | Adição ou ajuste de testes |
| `chore`    | Manutenção do projeto |
| `perf`     | Melhoria de performance |
| `ci`       | Alterações em pipelines e workflows |
| `build`    | Mudanças em build ou dependências |

---

## 🎯 3. Escopos (Opcional, Recomendado)

O escopo define **onde** a mudança foi aplicada.

### Exemplos de Escopos
- `auth`
- `api`
- `ui`
- `database`
- `config`
- `cart`
- `checkout`
- `payment`

### Exemplo com Escopo

`fix(api): handle null response from payment service (#22)`

---

## 🔄 4. Fluxo de Trabalho

1. Criar uma issue
2. Criar a branch conforme o padrão
3. Realizar commits pequenos, claros e semânticos
4. Abrir Pull Request com título no padrão Conventional Commits
5. Revisão de código
6. Merge para `main` ou `develop`

---

## 🧪 5. Exemplo Completo (Issue #15)

### Branch

`feat/15-add-login-form`

### Commits

`feat(auth): add login form layout (#15)`
`fix(auth): display error message on invalid credentials (#15)`

### Pull Request

`feat(auth): add login form with authentication (#15)`

---

## 📎 6. Resumo Rápido

### Branch

`<tipo>/<issue>-<descricao>`

### Commit

`<tipo>(escopo): descricao (#issue)`

### Exemplo Final

`feat(cart): add item quantity selector (#42)`

