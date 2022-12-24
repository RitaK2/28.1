В репозитории находится итоговый проект по курсу "Тестировщик-автоматизатор на Python" от SkillFactory. Объект тестирования: Авторизации/Регистрации/Восстановления страниц личного кабинета Росстелеком. Ссылка на ЛК Ростелеком: https://b2c.passport.rt.ru

По заданию тестирования необходимо:

Протестировать требования.

Разработать тест-кейсы (не менее 15). Необходимо применить несколько техник тест-дизайна.

Провести обеспеченность тестированием продукта (не менее 15 автотестов). Заказчик ожидает по одному автотесту на каждый письменный тест-кейс. Оформите свой набор автотестов на GitHub.

Оформить описание обнаруженных дефектов. Во время обучения вы работали с текстурами, сервисами и шаблонами, викоризовали их для оформления тест-кейсов и обнаружили дефекты. (если дефекты не обнаруживаются, необходимо описать дефект триа)

С тест-кейсами и описанными ошибками/дефектами/недостатками можно ознакомиться по ссылке: https://docs.google.com/spreadsheets/d/1CZ9MzW8fr0pgTr9hkEnzC8xUXWVsj6O8A7RjJznYjP8/edit?usp=sharing

Проект выполнен с помощью библиотеки Pytest и Selenium

Все тесты находятся в папке с тестами, файл test_rostelecom.py

Так же в папке test находится файл consts, тестовые данные и локаторы

При тестировании применялись такие техники тест-дизайна как: Проверка граничных значений, эквивалентное разделение, предугадывание ошибок, исследовательское тестирование.

Сценарии работы автотестов:

Несколько тестов проверяют редирект по клику на страницы: Регистрация нового пользователя, Восстановление пароля, Пользовательского порога, авторизация при помощи аккаунта VK, авторизация при помощи OK аккаунта, авторизация при помощи Mail аккаунта, авторизация при помощи Google аккаунта, авторизация при помощи Яндекс аккаунта, чат Telegram, чат Viber
Проверка корректного изменения поля ввода логина в соответствии с выбранным табом
Корректно проходит проверку типа логина (мобильный телефон, почта, логин, личный счёт) в автоматическом режиме
Несколько проверок, проверяющих обнаружение ошибок при вводе данных Автором на страницу Регистрации
На странице Восстановления пароля так же проверены обновление капчи и работоспособность кнопки Вернуться назад
Для работы автотестов необходимы библиотеки Pytest и Selenium. В проекте WebDriver Selenium для Chrome 109 версии, что запущены тесты. Запустить тесты можно через терминал прописав последовательно: "cd FinalProject/tests" и "pytest". Или в PyCharm через кнопку Run.
