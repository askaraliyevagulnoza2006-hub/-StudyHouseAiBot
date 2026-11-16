import telebot

TOKEN = "BU_YERGA_BOT_TOKENINGNI_QO'Y"

bot = telebot.TeleBot(TOKEN)

@bot.message_handler(commands=['start'])
def start(message):
    bot.reply_to(
        message,
        "Assalomu alaykum! 👋\n"
        "StudyHouse botiga xush kelibsiz! 📚\n"
        "Sizga qanday yordam bera olaman?"
    )

bot.infinity_polling()# -StudyHouseAiBot
