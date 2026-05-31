# Convenção de Branches

## Estrutura padrão de branches

### Fluxo

```text
feat/* -> dev -> main
```

### Main

Branch principal do repositório

#### Finalidade

- Armazenar versão estável do projeto
- Representa estado oficial do projeto

#### Regras

- `Require a pull request before merging`
- `Required approvals` - (Uma aprovação por padrão)
- `Dismiss stale pull request approvals`
- `Require conversation resolution before merging`
- `Require linear history`
- `Do not allow bypassing the above settings`
- `Restrict who can push to matching branches`

---

### Dev

Branch de integração e validação

#### Finalidade

- Consolidar e testar funcionalidades desenvolvidas pela equipe
- Realizar testes integrados
- Validar entregas antes de entrarem em produção

#### Regras

- `Require a pull request before merging`
- `Required approvals` - (Uma aprovação por padrão)
- `Dismiss stale pull request approvals`
- `Require conversation resolution before merging`
- `Require linear history`
- `Do not allow bypassing the above settings`
- `Restrict who can push to matching branches`

---

### Feature Branches (feat/*)

Branches para desenvolvimento de funcionalidades específicas

#### Finalidade

- Isolar o desenvolvimento de cada Story
- Permitir desenvolvimento paralelo
- Facilitar revisão e rastreabilidade de código

#### Convenção de nome

```text
feat/A2A-XXX-descricao

A2A - Prefixo do Jira
XXX - Número da story / task / subtask
descricao - Resumo da story em no máximo três palavras
```

##### Exemplos

```text
feat/A2A-26-login
feat/A2A-51-acessibilidade-wcag
```

#### Regras
- `Allow force pushes`
- `Allow deletions`