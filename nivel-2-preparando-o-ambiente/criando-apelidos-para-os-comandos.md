# Criando Apelidos para os Comandos

## Git Aliases

Git aliases são atalhos que você pode criar para comandos Git que usa com frequência. Por exemplo, em vez de digitar git status toda hora, você pode criar um alias git st.

### Exemplo: Criando o alias `st` para o comando `status`:

Para definir utilizar o comando  `git st` para acionar o  `git status`, podemos configurar um alias da seguinte maneira:

```bash
git config --global alias.st status
```

### Exemplo: Removendo o alias `st`:

Para remover o alias que criamos, utilizamos o seguinte comando:

```bash
git config --global --unset alias.st
```
