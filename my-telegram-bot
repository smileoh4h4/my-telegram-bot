const TelegramBot = require('node-telegram-bot-api');
const token = '7737037687:AAHvgpRoETlszHHHBZtR0zs9jEQe9tCfzVs';  // 把 YOUR_BOT_API_TOKEN 換成你的 Bot Token
const bot = new TelegramBot(token, { polling: true });

// 收到 /start 指令時的回應
bot.onText(/\/start/, (msg) => {
    const chatId = msg.chat.id;
    bot.sendMessage(chatId, '歡迎來到我的 Telegram Bot！');
});

// 回應所有訊息
bot.on('message', (msg) => {
    const chatId = msg.chat.id;
    bot.sendMessage(chatId, `你說的是: ${msg.text}`);
});
