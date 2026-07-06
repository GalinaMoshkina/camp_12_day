# Лагерь Эметар

Статический сайт для GitHub Pages. Telegram-бот и Python-сервер больше не используются.

Счетчик ключей хранится в браузере через `localStorage`. Это значит, что на каждом устройстве будет свой счетчик. Для экрана мероприятия открой сайт на том компьютере, который показывает проектор, и добавляй ключи через маленькую кнопку в правом нижнем углу.

## Локальный просмотр

Можно просто открыть `index.html` в браузере.

Если хочешь запустить через локальный сервер:

```bash
cd /home/gala/.vscode/2course/camp/12_day_web
python3 -m http.server 8000
```

Затем открыть:

```text
http://localhost:8000
```

## Как пользоваться

1. Открой сайт.
2. Нажми на маленькую кнопку в правом нижнем углу.
3. Введи количество новых ключей.
4. Нажми `Добавить`.

Каждые 35 ключей открывают одну коробку. Всего коробок: 30.

## Как загрузить в новый GitHub-репозиторий

Репозиторий: `https://github.com/GalinaMoshkina/camp_12_day.git`

Из папки проекта выполни:

```bash
cd /home/gala/.vscode/2course/camp/12_day_web
git init
git branch -M main
git add index.html background.png README.md .gitignore
git commit -m "Create static camp site"
git remote add origin https://github.com/GalinaMoshkina/camp_12_day.git
git push -u origin main
```

Если GitHub скажет, что remote уже существует:

```bash
git remote set-url origin https://github.com/GalinaMoshkina/camp_12_day.git
git push -u origin main
```

## Как включить GitHub Pages

1. Открой репозиторий на GitHub.
2. Зайди в `Settings`.
3. Открой раздел `Pages`.
4. В `Build and deployment` выбери:
   - `Source`: `Deploy from a branch`
   - `Branch`: `main`
   - папка: `/root`
5. Нажми `Save`.

Через пару минут сайт будет доступен примерно по адресу:

```text
https://galinamoshkina.github.io/camp_12_day/
```
