import telebot

bot = telebot.TeleBot("1215747770:AAGDCDf9YMzFOILyd6os7x5p8EF7yGN7dSw")

@bot.message_handler(commands=['start', 'help'])
def send_welcome(message):
	bot.reply_to(message, "ciao, come stai?")
