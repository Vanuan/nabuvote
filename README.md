    National Anti-Corruption Bureau of Ukraine
    E-Voting System for Public Control Council
    Complies TU U 58.29.4-39582446-001:2015 v1
    Copyright NGO E-DEMOCRACY http://ed.org.ua

    For further information, please contact us
    via e-mail <info@ed.org.ua>

    Next text in Russian only in UTF-8 charset
    try use translate.google.com if necessary



## Система рейтингового интернет голосования

Появилась где-то между 5 и 10 часами вечера 26 мая 2015 года, как
альтернатива существующей тогда системе выборов Общественного совета
при Национальном антикоррупционном бюро Украины (http://nabu.gov.ua).


## Используемые проверки и ограничения

Для предотвращения автоматического и повторного голосования в системе
используются следующие проверки:

1. Анти-робот тест (используется Google reCAPTCHA)
2. Проверка адреса электронной почты с вводом кода проверки из письма
3. Проверка номера мобильного телефона с получением кода в SMS

#### Пользовательские ограничения

1. Общее ограничение на время одной сессии: от теста reCAPTCHA до выбора
кандидатов не более 15 минут.
2. Ограничение на общее количество POST запросов в рамках одной сессии.
3. Ограничение на количество попыток ввода кодов проверки e-mail и
номера мобильного телефона.
4. Номер телефона и адрес электронной почты можно использовать только
для одного голосования.


## Открытый файл протокола голосования

Частично анонимизированные данные проголосовавших с указанием выбранных
кандидатов доступны в режиме on-line.


## Принципы разработки

Невероятно сжатые сроки разработки и необходимость прохождения аудита
безопасности для использования в государственных органах привели к выбору
следующих принципов построения системы:

- Отказ от универсальных решений
- Решение только задачи выборов Общественного совета НАБ Украины
- Минимальное количество доступного для аудита кода
- Минимальное использование дополнительных библиотек
- Отказ от использования фреймворков на стороне сервера
- Поддержка мобильных устройств и адаптивная верстка
- Защита от известных XSS и CSRF атак
- Защита от инъекций в пользовательских данных
- Подключение к базе данных только при необходимости

При отправке замечаний к коду пожалуйста учитывайте эти требования.


## Системные требования

- PHP >= 5.3
- MySQL >= 4.1
- php-mysqli
- php-curl


## Установка

1. Распакуйте архив в папку доступную веб-серверу
2. Создайте или подготовьте базу данных MySQL
3. Переименуйте settings.example.php в settings.php
4. Заполните недостающие значения в settings.php
5. Запустите из командной строки php install.php
6. При необходимости отредактируйте candidates.php
7. После завершения установки удалите install.php


## Аудит исходного кода

Передана на базовый аудит в Государственную службу специальной связи и защиты информации Украины. Результаты аудита не известны.

Аудит исходного кода приветствуется. Замечания присылайте на адрес
указанный ниже. Пожалуйста учитывайте принципы разработки описанные выше - это не универсальная система.


## Лицензия

В рамках Меморандума о сотрудничестве передана для использования
в рамках выборов Общественного совета при Национальном антикоррупционном бюро Украины.

Для использования в других официальных выборах обращайтесь по контактам приведенным ниже.


## Контакты

Общественная организация
"Электронная демократия"

http://ed.org.ua/

info@ed.org.ua






