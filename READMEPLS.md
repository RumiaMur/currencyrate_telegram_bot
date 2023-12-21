# Telegram-бот для мониторинга погоды

Telegram-бот, что позволяет отслеживать изменения в погодных условиях. Пользователи могут настроить бота для отслеживания определенных городов, узнавать конкретное значение температуры в конкретные периоды времени.

## Функции бота

- Выбор города для отселживания: выберите нужный Вам город для мониторинга погоды
- График температур: Отслеживайте изменения в температуре
Что у нас вообще еще делает бот?

## Предварительные условия

Перед запуском бота убедитесь, что у вас установлены следующие зависимости:

- Python 3.x
- Pip 22.x.x
- Необходимые библиотеки Python (см. requirements.txt) 

## Установка

1. Клонируем репозиторий:

        git clone https://github.com/TenshiDT/TRPO_tg_bot
        cd TRPO_tg_bot

2. Устанавливаем зависимости:

        pip install -r requirements.txt

3. Настройка ключей API:

- Создайте Telegram-бота через [@BotFather](https://t.me/BotFather) и получите ключ API
- Получите ключ API из сервиса [WTTR.in](https://wttr.in/) для данных о погоде - а у нас это есть вообще api key тута? И в 4 пункте тоже тот же вопрос про api key 

4. Создайте файл .env в корне проекта и добавьте свои API-ключи:

        API_KEY_BOT="telegram_bot_api_key"
        API_KEY_LAYER="currency_api_layer_key"

5. Запустите бота:

        python main.py

## Использование

1. Запустите бота, отправив /start, чтобы инициировать процесс настройки
2. Используйте /settings для настройки параметров мониторинга
3. Следуйте инструкциям бота, чтобы установить валюту, интервал мониторинга и пороговые значения
4. Запустите мониторинг с помощью /monitor
5. Проверьте последний курс валюты с помощью /currency
6. Отмените мониторинг с помощью /cancel в любое время