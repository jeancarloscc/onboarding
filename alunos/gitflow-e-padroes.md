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

A mensagem de commit deve seguir a seguinte regra: \
`#[número da issue] - [mensagem de commit]`

Exemplos de mensagem de commits numa branch para realizar a issue 42:

```
#42 - Criação da tela de login
#42 - Inclusão do botão de recuperação de senha
#42 - Alteração da lógica de checagem de email válido
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

### Vinculação da Issue

- Ao abrir um Pull Request, utilize o campo **Development**, disponível na própria tela de criação/edição do PR.
- Nesse campo, associe a issue relacionada à sua entrega.
- Quando o vínculo é feito corretamente, ao mergear o PR, a issue vinculada será encerrada automaticamente.
---

### Processo de revisão

- Recomenda-se que todo Pull Request seja revisado por pelo menos 1 membro da equipe antes do merge.
- Ao receber comentários ou solicitações de correção, responda e/ou atualize o PR, se necessário.
- Essa etapa de revisão contribui para a qualidade do código, compartilhamento de conhecimento e padronização do projeto.
- No entanto, **a adoção desse processo fica a critério da liderança da equipe**, que pode definir se haverá (ou não) a etapa de revisão no projeto.