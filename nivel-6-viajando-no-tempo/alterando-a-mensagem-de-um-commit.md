# Alterando a Mensagem de um Commit

O comando `git commit --amend` permite alterar o último commit que você fez. Para modificar a mensagem do commit diretamente, sem abrir o editor, utilize o comando:

```bash
git commit --amend –m"nova mensagem"
```

Quando você usa `git commit --amend`, o Git substitui o último commit por um novo, criando um novo hash. Isso significa que o commit original deixa de estar na branch atual, mas ele não desaparece imediatamente.

> O comando `git reflog` mantém um histórico de todas as mudanças do ponteiro HEAD, incluindo commits antigos, rebases, resets e também commits alterados por amend.
