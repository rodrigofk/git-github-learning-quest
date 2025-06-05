# Desfazendo um Commit

## Git Reset

O comando `git reset` serve para mover o ponteiro do HEAD para um commit específico, alterando opcionalmente o índice (staging area) e o diretório de trabalho. Dependendo da opção usada, ele pode desfazer commits, modificar o que está preparado para commit ou até apagar mudanças locais.

### Exemplo:

Suponha que você queira desfazer o último commit:

`git reset --soft HEAD~1` — desfaz o commit, mantém tudo staged (pronto para commit).

`git reset --mixed HEAD~1` _(comportamento padrão_ `git reset HEAD~1`_)_ — desfaz o commit e remove do staging, mas mantém arquivos alterados.

`git reset --hard HEAD~1` — desfaz o commit e apaga todas as alterações locais (⚠️ use com cautela).
