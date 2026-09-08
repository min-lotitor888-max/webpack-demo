# webpack-demo
## Статус
Готово к проверке.

## Репозиторий
[https://github.com/neo/webpack-demo](https://github.com/min-lotitor888-max/webpack-demo.git)

## Описание
Реализована модульная структура приложения:
- Модуль Domain: `src/js/domain.js` (класс Character, default export).
- Модуль Game: `src/js/game.js` (класс Game, GameSavingData, функции read/writeGameSaving).
- Модуль App: `src/js/app.js` (импорт Game, переименование функций в loadGame/saveGame).

Настроена сборка Webpack:
- Entry point: `src/index.js`.
- HTMLWebpackPlugin для генерации `index.html`.
- MiniCssExtractPlugin для выделения CSS.
- Скрипты в package.json: `build`, `start`, `serve-dist`.

## Проверка
1. `npm run build` — сборка в папку `dist`.
2. `npm run serve-dist` — запуск HTTP‑сервера для проверки собранного бандла (отдаёт содержимое папки `dist`).
3. В консоли браузера ожидается: `app worked` и `game started`.
4. Цвет текста на странице — серый (`body { color: #999; }`).
