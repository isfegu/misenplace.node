# Mise en place, node

Este repositorio contiene la base para empezar el desarrollo de un proyecto basado en:

- [Node.js](https://nodejs.org/es/)
- [Typescript](https://www.typescriptlang.org) o Javascript

Utilizando como entorno de desarrollo:

- [Visual Studio Code](https://code.visualstudio.com/)
- [Remote Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

## Descripción

Este proyecto instala y configura las siguientes herramientas:

- [Prettier](https://prettier.io): Para validar el formato del código Javscript o Typescript. Puedes ver la configuración en los archivos [.prettierrc](.prettierrc) y [.prettierignore](.prettierignore)
- [ESLint](https://eslint.org/): Para buscar y corregir problemas en el código Javascript o Typescript. Puedes ver la configuración en el archivo [.eslintrc.json](.eslintrc.json)
- [Commitlint](https://commitlint.js.org/): Para validar que los mensajes de commit sigan las directrices de [Conventional Commits](https://www.conventionalcommits.org). Puedes ver la configuración en el archivo [commitlint.config.js](commitlint.config.js)
- [Husky](https://typicode.github.io/): Para gestiona cómodamente los Git Hooks. Los git hooks configurados son:
  - _pre-commit_: Ejecuta ESLint y Prettier
  - _commit-msg_: Ejecuta Commitlint

## Uso

Para usar este proyecto como base de tu proyecto, puedes o clonar este repositorio o descárgalo. Luego debes adaptarlo a tus necesidades.

### Instalar los requisitos

1. [Docker](https://docs.docker.com/get-docker/)
2. [Visual Studio Code](https://code.visualstudio.com/)
3. [Remote Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers).

### Iniciar el entorno

Abre este proyecto (o el _[workspace](misenplace.node.code-workspace)_) en [Visual Studio Code usando el contenedor remoto](https://code.visualstudio.com/docs/remote/containers).

> La primera vez que abras este proyecto tomará más tiempo ya que debe descargarse la imagen docker y construir el contenedor.

### Instalar las dependencias

Abre una terminal desde dentro de Visual Studio Code y ejecuta:

```bash
node ➜ /workspaces/misenplace.node (main) $ yarn
```

### Adáptalo

La configuración que traen [Prettier](.prettierrc), [ESlint]((.eslintrc.json), [Commitlint]((commitlint.config.js) y [Husky](./.husky) están a modo de ejemplo, adáptalo a tus necesidades.

## Contribuir

Si encuentras útil este proyecto y quieres aportar tu granito de arena en mejorarlo, haz un _pull request_ con tu contribución, usando:

- El entorno que este mismo proyecto proporciona
- [Conventional Commits](https://www.conventionalcommits.org)

Muchas gracias de antemano.
