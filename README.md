# 🌐 GK-Localization for Clickteam Fusion 2.5
Система локализации, построенная на работе с JSON-файлами. Поддерживает чтение внешних файлов, встраивание файлов в бинарную дату. Работает на Windows, Android, HTML5. Пример строения JSON-файла предоставлен в папке `languages`. Рекомендуется использовать приложения или сервисы для создания JSON-локализаций.

💡 *Разработано для игр GKProduction, но может использоваться в ваших проектах.*

![GK-Localization](icon.png)

## Как добавить систему в свой проект
- Добавить фрейм «Выбор языка» в свой проект;
- Добавить объекты из фрейма «Служебное» или сам фрейм в свой проект;
- Добавить группу событий "Загрузка локализации v5" (находится в глобальных событиях) в свой проект.
## Как встроить языки в игру
Подойдёт для Windows и Android. Могло бы подойти для HTML5, если бы не проблема невозможности сменить кодировку у Edit Box.
- Добавить в бинарные данные проекта все файлы языков;
- Укажите путь к бинарным файлам во фрейме «Выбор языка» в событиях `20` для Windows и в `22` для Android;
- Заполните список «Файлы языков» названиями файлов языков (находится на фрейме).
## Как иметь языки во внешних файлах
Подойдёт для Windows.
- Создайте папку `languages` рядом с mfa/exe (путь можно изменить во фрейме «Выбор языка» в событии `15`);
- Поместите туда все файлы языков.
## Если выпускаете приложение для HTML5
Подойдёт для HTML5.
- Создайте папку `languages` рядом с `index.html` (путь можно изменить во фрейме «Выбор языка» в событии `24`);
- Подключите к игре скрипты CallbackCatcher, GetLanguage и GetLocalization (читайте `For HTML5\README.md`, чтобы узнать больше).

Остальные вещи описаны в самом исходном коде в специальных сносках.

Вы можете посмотреть, как работает система, [здесь](https://gkproduction.github.io/web_games/supa_dupa_game/index.html).

## Требования
- Clickteam Fusion 2.5 версии R295.10 и выше
- Clickteam Fusion 2.5+
- Clickteam Fusion 2.5 Developer
- Clickteam Fusion 2.5 - Android Exporter
- Clickteam Fusion 2.5 - HTML5 Exporter

## Требуемые расширения
- JSON Object
- String Tokenizer
