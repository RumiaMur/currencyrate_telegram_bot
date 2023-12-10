# Telegram-бот для мониторинга валют

Данный Telegram-бот предназначен для мониторинга курсов обмена валют. Пользователи могут настроить бота для отслеживания определенных валют, устанавливать интервалы мониторинга и получать уведомления на основе пороговых значений.

## Функции

- Выбор валюты: Выберите валюту для мониторинга (например, EUR, USD, JPY)
- Настройка интервала: Установите интервал мониторинга в минутах
- Пороговые оповещения: Получайте уведомления, когда курс валюты выходит за указанные пороговые значения
- Графическое представление: Просматривайте исторические курсы валют с помощью графических графиков

## Предварительные условия

Перед запуском бота убедитесь, что у вас установлены следующие зависимости:

- Python 3.x
- Необходимые библиотеки Python (см. requirements.txt)

## Установка

1. Клонируем репозиторий:

        git clone https://github.com/kamiamon/currencyrate_telegram_bot.git
        cd currencyrate_telegram_bot

2. Устанавливаем зависимости:

        pip install -r requirements.txt

3. Настройка ключей API:

- Создайте Telegram-бота через @BotFather и получите ключ API
- Получите ключ API из сервиса [API Layer](https://apilayer.com/marketplace/currency_data-api) для данных о валюте

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
