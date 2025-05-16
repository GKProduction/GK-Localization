К веб-игре должны быть подключены скрипты:
- CallbackCatcher.js (чтобы можно было получать ответы функций)
- GetLanguage.js (для авто-определения языка)
- GetLocalization.js (для чтения файла локализации)

Добавьте этот код в свой `index.html`, чтобы подключить скрипты:
``` html
	<!-- Возвращение ответов функций для модуля Collection of API -->
	<script src="scripts/CallbackCatcher.js"></script>
	
	<!-- Получить язык браузера -->
	<script src="scripts/GetLanguage.js"></script>
	
	<!-- Получить файл локализации -->
	<script src="scripts/GetLocalization.js"></script>
```
Скрипты должны лежать в папке `scripts` рядом с `index.html`. Путь можно изменить.
