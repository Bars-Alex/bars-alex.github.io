# Website

This website is built using [Docusaurus](https://docusaurus.io/), a modern static website generator.

## Installation

```bash
yarn
```

## Local Development

```bash
yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

## Build

```bash
yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

## Deployment

Using SSH:

```bash
USE_SSH=true yarn deploy
```

Not using SSH:

```bash
GIT_USER=<Your GitHub username> yarn deploy
```
Исходный код моего сайта.

https://bars-alex.github.io

/blog/ — содержит файлы блога в формате Markdown. Вы можете удалить каталог, если отключили плагин блога, или изменить его название после настройки параметра path . Более подробную информацию можно найти в руководстве по блогу

/docs/ — содержит файлы Markdown для документации. Настройте порядок отображения боковой панели документации в sidebars.js. Вы можете удалить каталог, если отключили плагин документации, или изменить его название после настройки параметра path . Более подробную информацию можно найти в руководстве по документации

/src/ - Файлы, не относящиеся к документации, например страницы или пользовательские React-компоненты. Вам не обязательно размещать здесь файлы, не относящиеся к документации, но если они будут находиться в централизованном каталоге, их будет проще указать в случае необходимости какой-либо проверки или обработки

/src/pages - Любой файл JSX/TSX/MDX в этом каталоге будет преобразован в страницу сайта. Более подробную информацию можно найти в руководстве по страницам

/static/ - Статический каталог. Все его содержимое будет скопировано в корень итогового build каталога

/docusaurus.config.js - Файл конфигурации, содержащий настройки сайта. Это аналог siteConfig.js в Docusaurus v1

/package.json - Сайт на Docusaurus — это React-приложение. В него можно устанавливать и использовать любые пакеты npm.

/sidebars.js - Используется в документации для указания порядка документов на боковой панели

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.
