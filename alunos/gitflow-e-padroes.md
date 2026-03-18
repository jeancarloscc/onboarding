# 📁 GitFlow — Organização do Código

Os repositórios dos projetos do Laboratório de Inteligência de Dados devem seguir o modelo **GitFlow**, com as seguintes convenções para facilitar a colaboração e manter a consistência.

---

## Principais branches

| Branch        | Descrição                                             |
|---------------|--------------------------------------------------------|
| `main`        | Código estável e em produção                             |
| `develop`     | Integração de funcionalidades em desenvolvimento         |
| `feature-*`   | Desenvolvimento de novas funcionalidades                |
| `hotfix-*`    | Correções de bugs                                       |

---

## Padrão de nomes de branches

Utilize o prefixo da categoria seguido do número da issue relacionada e um nome descritivo em `kebab-case`:

```
feature-42-login-tela
hotfix-50-erro-validacao-formulario
```
---

## Padrão de mensagens de commits

A mensagem de commit deve seguir o padrão **Conventional Commits**, amplamente adotado por equipes profissionais.

Formato recomendado:

```
tipo: descrição curta no imperativo
```

Tipos mais usados:

- `feat`: adiciona uma nova funcionalidade.
- `fix`: corrige um bug.
- `docs`: altera documentação (sem mudar código).
- `test`: cria ou ajusta testes (sem mudar regra de negócio).
- `build`: altera build ou dependências.
- `perf`: melhora performance.
- `style`: ajusta formatação/lint (sem mudar comportamento).
- `refactor`: reorganiza código sem alterar funcionalidade.
- `chore`: tarefa de manutenção/configuração.
- `ci`: altera pipeline de integração contínua.
- `raw`: altera arquivos brutos de configuração/dados/parâmetros.
- `cleanup`: limpa código desnecessário.
- `remove`: remove arquivos, código ou funcionalidades obsoletas.

Boas práticas:

- Use descrição curta, clara e objetiva.
- Prefira um commit por mudança lógica.
- Evite mensagens genéricas como "ajustes" ou "update".

Exemplos de commits:

```
feat: cria tela de login
fix: corrige validação de e-mail
docs: atualiza instruções de execução
refactor: simplifica tratamento de erros
test: adiciona testes para cadastro
chore: atualiza dependências do projeto
ci: ajusta pipeline de integração contínua
build: atualiza configuração de build
perf: otimiza consulta de dados
style: aplica padronização de lint e formatação
cleanup: remove código comentado
remove: exclui módulo legado descontinuado
```
---

## Pull Requests

### Título do PR

Use o padrão:

```
[feature] Cria tela de login
[hotfix] Corrige validação do formulário
```

> O prefixo entre colchetes indica o tipo da entrega.

### Descrição do PR

- Faça um resumo do que foi entregue.

### Vinculação com o Trello

- Adicione no PR o link do cartão correspondente no Trello.
- No cartão do Trello, inclua o link do PR para facilitar o acompanhamento.
- Atualize a lista do cartão conforme o andamento: **In Review** durante a revisão e **Concluído** após o merge.
---

### Processo de revisão

- Recomenda-se que todo Pull Request seja revisado por pelo menos 1 membro da equipe antes do merge.
- Ao receber comentários ou solicitações de correção, responda e/ou atualize o PR, se necessário.
- Essa etapa contribui para a qualidade do código, compartilhamento de conhecimento e padronização do projeto.
- No entanto, **a adoção desse processo fica a critério da liderança da equipe**, que pode definir se haverá (ou não) a etapa de revisão no projeto.