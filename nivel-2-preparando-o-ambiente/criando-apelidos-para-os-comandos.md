# Criando Apelidos para os Comandos

### Git Aliases: Adicionando apelidos para os comandos do Git

Exemplo: Criando um alias para o comando `status`:

```bash
$ git config --global alias.st status
```

Agora podemos utilizar o comando  `git st` para acionar o  `git status`.\
Para remover o alias que criamos, utilizamos o seguinte comando:

```bash
$ git config --global --unset alias.st
```

