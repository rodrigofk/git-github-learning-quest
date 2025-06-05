# Configurando o Git

O Git armazena suas configurações em arquivos de configuração em diferentes níveis. Cada nível tem sua própria localização e prioridade.

Ao especificar a opção `--local`, `--global` ou `--system` com o comando git config, você informa em qual nível deseja salvar ou consultar a configuração:

<table><thead><tr><th width="106.33334350585938">Escopo</th><th width="121">Opção</th><th>Afeta</th><th>Localização do arquivo</th></tr></thead><tbody><tr><td><strong>Local</strong></td><td><code>--local</code></td><td>Só o repositório atual</td><td><code>.git/config</code> dentro do repositório</td></tr><tr><td><strong>Global</strong></td><td><code>--global</code></td><td>Todos os repositórios do usuário</td><td><code>~/.gitconfig</code> (Linux/macOS) ou <code>%USERPROFILE%\.gitconfig</code> (Windows)</td></tr><tr><td><strong>System</strong></td><td><code>--system</code></td><td>Todos os usuários da máquina</td><td><code>/etc/gitconfig</code> (Linux) ou pasta de instalação do Git (Windows)</td></tr></tbody></table>

Se nenhuma dessas opções for usada, o Git aplica a configuração no nível local por padrão, desde que esteja dentro de um repositório.

Para visualizar as configurações ativas, utilize o comando:

```bash
git config --list
```

Para visualizar as configurações com o caminho do arquivo onde estão definidas, use:

```bash
git config --list --show-origin
```

## Configurações Básicas&#x20;

### Nome de usuário

```bash
git config --global user.name "Nome Sobrenome"
```

### &#x20;E-mail&#x20;

```bash
git config --global user.email seuemail@email.com
```

### Branch Padrão

Para definir o nome padrão da branch principal para "**main**" ao criar novos repositórios com `git init`, utilize o comando:

```bash
git config --global init.defaultBranch main
```
