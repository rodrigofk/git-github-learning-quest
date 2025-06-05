# O que é Versionamento de Código?

Versionamento de código é uma forma de controlar e registrar todas as alterações feitas no código de um projeto ao longo do tempo — sem precisar criar cópias manualmente. Com ele, é possível salvar versões anteriores, voltar atrás em caso de erro, acompanhar quem fez cada modificação e permitir que várias pessoas trabalhem juntas sem conflitos.

## Sistemas de Controle de Versão

Os Sistemas de Controle de Versão (Version Control System - VCS), são softwares que controlam as versões de um arquivo ao longo do tempo. Eles permitem:

* 🕒 Registrar o histórico de atualizações de um arquivo
* 🔁 Voltar no tempo (para uma versão anterior se algo der errado)
* 🤝 Colaborar com outras pessoas sem bagunça
* 🔍 Saber quem alterou o quê, quando e por quê

| Sistemas                | Descrição                                                                    | Exemplos                                                                                                                                                                  |
| ----------------------- | ---------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Centralizado (CVCS)** | Um único servidor dispõe dos arquivos de controle de versão.                 | ![CVS](https://img.shields.io/badge/CVS-000?style=for-the-badge\&logo=cvs)![Subversion](https://img.shields.io/badge/Subversion-000?style=for-the-badge\&logo=subversion) |
| **Distribuído (DVCS)**  | Duplica localmente o repositório completo, incluindo o histórico de versões. | ![Git](https://img.shields.io/badge/Git-000?style=for-the-badge\&logo=git)![Mercurial](https://img.shields.io/badge/Mercurial-000?style=for-the-badge\&logo=mercurial)    |

## Versionamento Semântico

O padrão conhecido como **Versionamento Semântico (SemVer)** usa três números para indicar o tipo de atualização, no formato MAJOR.MINOR.PATCH.

* **MAJOR:** Mudanças incompatíveis com versões anteriores.
* **MINOR:** Novas funcionalidades compatíveis com versões anteriores.
* **PATCH:** Correções de bugs ou pequenas melhorias, sem impacto em funcionalidades.

> #### Exemplo prático:
>
> Se a sua versão é 2.1.3 e você lançou um grande recurso novo sem quebrar nada, a versão vai para 2.2.0 (o patch é resetado para 0, pois uma nova versão está sendo lançada). Se depois você fizer uma correção, a versão vai para 2.2.1.

Entenda mais sobre o padrão SemVer em: [semver.org](https://semver.org)
