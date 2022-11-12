# tg-bot


import telebot
from tk import *

bot = telebot.TeleBot(token)


@bot.message_handler(content_types=['text'])
def text(message):
    if message.text == 'Привет':
        bot.send_message(message.from_user.id, 'Приветствую тебя мой дорогой друг')
    elif message.text == 'Как дела':
        bot.send_message(message.from_user.id, 'Всё замечательно')
    elif message.text == 'Можешь записать меня':
        bot.send_message(message.from_user.id, 'перейди по ссылке https://b211998.yclients.com/company/211188/select-services?referrer=https:%2F%2Fwww.residentmen.ru%2F&o=m2055588')
    elif message.text == 'Можешь записать меня на стрижку':
        bot.send_message(message.from_user.id, 'перейди по ссылке https://b211998.yclients.com/company/211188/select-services?referrer=https:%2F%2Fwww.residentmen.ru%2F&o=m2055588')
    elif message.text == 'Нужно подстричься':
        bot.send_message(message.from_user.id, 'перейди по ссылке https://b211998.yclients.com/company/211188/select-services?referrer=https:%2F%2Fwww.residentmen.ru%2F&o=m2055588')
    elif message.text == 'На сегодня есть время':
        bot.send_message(message.from_user.id, 'перейди по ссылке https://b211998.yclients.com/company/211188/select-services?referrer=https:%2F%2Fwww.residentmen.ru%2F&o=m2055588')
    elif message.text == 'На сегодня есть местечко':
        bot.send_message(message.from_user.id, 'перейди по ссылке https://b211998.yclients.com/company/211188/select-services?referrer=https:%2F%2Fwww.residentmen.ru%2F&o=m2055588')
    elif message.text == 'Запиши меня':
        bot.send_message(message.from_user.id, 'перейди по ссылке https://b211998.yclients.com/company/211188/select-services?referrer=https:%2F%2Fwww.residentmen.ru%2F&o=m2055588')
    elif message.text == 'Запиши меня на сегодня':
        bot.send_message(message.from_user.id, 'перейди по ссылке https://b211998.yclients.com/company/211188/select-services?referrer=https:%2F%2Fwww.residentmen.ru%2F&o=m2055588')
    else:
        bot.send_message(message.from_user.id, 'Я кажется знаю что тебе нужно,перейди по ссылке https://b211998.yclients.com/company/211188/select-services?referrer=https:%2F%2Fwww.residentmen.ru%2F&o=m2055588')

bot.infinity_polling()
