# Дипломная работа 'VKinder'

## Запуск программы
1. Устанавливаем требуемые библиотеки:
``` 
    pip install vk_api
    pip install psycopg2
```
2. Заполняем переменные в файле config.py --- [(<a href="https://vkhost.github.io/">Токен пользователя</a>), (<a href= "https://github.com/netology-code/py-advanced-diplom/blob/new_diplom/group_settings.md/">токен сообщества</a>)]
4. Запускаем файл bot.py
5. Взаимодействие с ботом начинается после нажатия кнопки 'Начать поиск' в чате с сообществом, чей токен (сomm_token) указан в файле config.py

## Задание
Все слышали про известное приложение для знакомств - Tinder. Приложение предоставляет простой интерфейс для выбора понравившегося человека. Сейчас в Google Play более 100 миллионов установок.

Используя данные из VK, нужно сделать сервис намного лучше, чем Tinder, а именно: чат-бота “VKinder”. Бот должен искать людей, подходящих под условия, на основании информации о пользователе из VK:

    Возраст,
    пол,
    город,
    семейное положение.

У тех людей, которые подошли по требованиям пользователю, получать топ-3 популярных фотографии профиля и отправлять их пользователю в чат вместе со ссылкой на найденного человека.
Популярность определяется по количеству лайков и комментариев.

За основу можно взять код из файла basic_code.py.
Как настроить группу и получить токен можно найти в инструкции.

Входные данные

    Имя пользователя или его id в ВК, для которого мы ищем пару.

если информации недостаточно нужно дополнительно спросить её у пользователя.

Требования к сервису:

    Код программы удовлетворяет PEP8.
    Получать токен от пользователя с нужными правами.
    Программа декомпозирована на функции/классы/модули/пакеты.
    Результат программы записывать в БД.
    Люди не должны повторяться при повторном поиске.
    Не запрещается использовать внешние библиотеки для vk.
