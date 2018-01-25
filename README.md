# Frontend for SPA «ПомойАвто»

It is a frontend for single page application. Reach JavaScript is present.

# Deploy on localhost

Example of frontend launch on Linux, Python 3.5:

```bash
cd static/
python3 -m http.server
```

Open page [127.0.0.1:8000](http://127.0.0.1:8000) in browser.

# Deploy on production server

[TODO. Deploy scripts will written later]

# Project Goals

The code is written for educational purposes. Training course for web-developers - [DEVMAN.org](https://devman.org)

Хьюстон, у нас проблемы. Не удается прикрутить форму регистрации к новому сайту «ПомойАвто». Это SPA - Single Page Application - и логика предполагается следующая:

   - пользователь указывает email и пароль
   - на сервер уходит AJAX запрос
   - сервер регистрирует пользователя и выдает cookies
   - фронтенд перенаправляет на страницу со списком автомобилей пользователя
   - фронтенд запрашивает данные у сервера

Звучит все просто, но отчего-то не работает. Разберись с этим. Найди и почини.

Особенности проекта:

- API живет на отдельном поддомене api.33_spa.devman.org в своем репозитории отдельном от фронтенда;
- Фронтенд пребывает в зачаточном состоянии. Пользователю пока не отображаются ошибки заполнения форм регистрации и авторизации.

Рекомендации:

- Инструменты разработчика Chrome DevTools должны помочь. Особенно вкладка Network и заголовки HTTP запросов/ответов. HTTPie тоже может оказаться полезным.
- Вкладка Application>Storage>Cookies в Chrome DevTools.
- Режим Инкогнито в браузере для сброса cookies перед началом тестирования.
- Разобраться с механизмом [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/Access_control_CORS).

Что может оказаться полезно:

   [RIOT Guid](http://riotjs.com/guide/)

