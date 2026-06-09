# Ice Courier

## Русский

**Ice Courier** - простая браузерная 2D-игра на JavaScript для экзамена по МДК 05.02. Игрок управляет зимним курьером, ловит падающие магические кристаллы и уворачивается от опасных ледяных плит.

Играть онлайн: https://c3rlchvuaw.github.io/Ice-Courier/

### Как запустить

Откройте `index.html` в браузере или запустите локальный сервер:

```bash
python3 -m http.server 8000
```

Затем перейдите на `http://localhost:8000/`.

### Управление

- `A` / `D` или стрелки влево/вправо - движение игрока.
- Мышь - перемещение игрока по горизонтали.
- `Restart` - запуск или перезапуск игры.

### Цель игры

Соберите 15 кристаллов, чтобы выиграть. При столкновении с ледяной плитой теряется 1 жизнь. Игра заканчивается поражением, когда жизни доходят до 0.

### Режимы

- **Цель: 15** - классический экзаменационный режим с победой после 15 кристаллов.
- **Рекорд** - бесконечный режим без ограничения по цели. Сложность растёт: объекты падают быстрее, ледяные плиты появляются чаще, а после набора очков возникают дополнительные волны.

### Особенности

- Canvas API и игровой цикл на `requestAnimationFrame`.
- Очки, жизни, цель, отдельные рекорды режимов через `localStorage`.
- Всплывающие подсказки `+1 очко` и `-1 жизнь`.
- Спрайт-лист игрока из 3 кадров.
- Локальные PNG-ассеты без внешних зависимостей.

### Использование нейросетей

- ChatGPT/Codex: идея, стартовая структура кода, рефакторинг и UI-доработки.
- OpenAI image generation: фон, спрайт-лист игрока, кристалл и ледяная плита.

### Проверка

Игра рассчитана на запуск в современных браузерах: Google Chrome, Mozilla Firefox и Microsoft Edge. В коде указано, что обязательная проверка проводилась для Chrome и Firefox.

---

## English

**Ice Courier** is a simple browser-based 2D JavaScript game created for an MDK 05.02 exam assignment. The player controls a winter courier, catches falling magic crystals, and avoids dangerous cracked ice rocks.

Play online: https://c3rlchvuaw.github.io/Ice-Courier/

### How to Run

Open `index.html` in a browser or start a local server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000/`.

### Controls

- `A` / `D` or left/right arrow keys - move the player.
- Mouse movement - move the player horizontally.
- `Restart` - start or restart the game.

### Goal

Collect 15 crystals to win. Hitting an ice rock removes 1 life. The game ends when the player has no lives left.

### Modes

- **Goal: 15** - the classic exam mode with a win condition after 15 collected crystals.
- **Record** - an endless high-score mode with no score limit. Difficulty increases over time: falling objects get faster, ice rocks become more frequent, and extra waves appear after the score grows.

### Features

- Canvas API with a `requestAnimationFrame` game loop.
- Score, lives, goal, and separate mode best scores stored with `localStorage`.
- Visual feedback for `+1 score` and `-1 life`.
- 3-frame player sprite sheet animation.
- Local PNG assets with no external runtime dependencies.

### AI Usage

- ChatGPT/Codex: game idea, starter code structure, refactoring, and UI improvements.
- OpenAI image generation: background, player sprite sheet, crystal, and ice rock obstacle.

### Browser Check

The game is designed for modern browsers: Google Chrome, Mozilla Firefox, and Microsoft Edge. The source comments state Chrome and Firefox as the required tested browsers.
