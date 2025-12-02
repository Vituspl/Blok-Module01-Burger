# Учебный проект Burger

Проект был выполнен в рамках базового курса по верстке от [Frontend Blok](https://frontendblok.com/).

**Ссылки по проекту**

- [Демо](https://vituspl.github.io/Blok-Module01-Burger/)

- [Макет Figma](https://www.figma.com/file/8muxUNt1PwGH5byQR6LZG8/Burgers-Menu-Responsive?node-id=0%3A1)

**Использованные технологии**

- HTML
- CSS (переменные, flexbox, grid)
- JavaScript

**Установки линтеров**

npm i -D eslint

npm i -D stylelint stylelint-config-standard

npm i -D prettier

**Внимание из-за особенностей Windows: потребовались дополнительные установки**

Нужно заменить ";" в двух последних скриптах для линтеров, долно получится:

"lint": "npm run lint:js && npm run lint:css",
"lint:fix": "npm run lint:js:fix && npm run lint:css:fix && npm run format"



Либо как вариант: Установить пакет: npm i -D npm-run-all

В package.json переписать два последних скрипта для линтеров, должно получиться:

"lint": "run-s lint:js lint:css",
"lint:fix": "run-s lint:js:fix lint:css:fix format"

**Конфигурации линтеров**

файл eslint.config.mjs - конфигурация eslinter;
файл stylelint.config.mjs - конфигурация stylelint;
файл .prettierc - конфигурация prettier;

**Запуск проверки линтерами**

npm run lint:fix - полная проверка с фиксами.

**Александр Ламков сделал и поделился стартовой сборкой для верстки, где в т.ч. и линтеры настроены. Большое ему спасибо!**

https://www.npmjs.com/package/friendly-frontend-lint-config

https://github.com/aleksanderlamkov/friendly-frontend-lint-config
