# Telegram и Discord Бот для Google Sheets

## Описание
Этот проект представляет собой бота, который интегрируется с Google Sheets, Telegram и Discord. Бот позволяет получать данные из Google Sheets и отправлять их в Telegram и Discord.

## Требования
- Node.js (рекомендуется версия 14.x и выше)
- npm (Node Package Manager)

## Установка
1. Клонируйте репозиторий:
    ```sh
    git clone https://github.com/IZenApp/TelegramWebhook.bot.git
    ```
2. Перейдите в директорию проекта:
    ```sh
    cd your-repo
    ```
3. Установите зависимости:
    ```sh
    npm install
    ```

## Использование
1. Запустите бота:
    ```sh
    node bot.js
    ```
2. Бот автоматически начнет опрашивать Telegram и отправлять данные в Discord.

## Конфигурация
1. **Google Sheets API**:
    - Создайте проект в [Google Cloud Console](https://console.cloud.google.com/).
    - Включите Google Sheets API.
    - Создайте учетные данные и скачайте JSON файл.
    - Поместите JSON файл в директорию `conf/` и назовите его `discordbot.json`.

2. **Telegram Bot**:
    - Создайте бота в Telegram через [BotFather](https://core.telegram.org/bots#botfather).
    - Получите токен и замените `botToken` в `bot.js`.

3. **Discord Webhook**:
    - Создайте вебхук в вашем Discord сервере.
    - Замените `discordWebhookUrl` в `bot.js`.

4. **Chat IDs**:
    - Создайте файл `chat_ids.json` в директории `conf/` и добавьте chat ID пользователей в формате JSON.

## Лицензия
Этот проект лицензирован под лицензией MIT. Подробности см. в файле [LICENSE](LICENSE).