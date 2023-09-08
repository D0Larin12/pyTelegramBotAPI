
===========
Quick start
from telebot import types
===========

.. meta::
   :description: Quickstart guide
   :keywords: ptba, pytba, pyTelegramBotAPI, quickstart, guide

Synchronous TeleBot bot = telebot.TeleBot('BOT-TOKEN')

$ pip установить pytelegrambotapi --обновить
-------------------
.. literalinclude:: ../../examples/echo_bot.py
    :language: python

Asynchronous TeleBot
--------------------
.. literalinclude:: ../../examples/asynchronous_telebot/echo_bot.py
    :language: python
 url(message):
    markup = types.InlineKeyboardMarkup()
    btn1 = types.InlineKeyboardButton(text='Наш сайт', url='https://habr.com/ru/all/')
    markup.add(btn1)
    bot.send_message(message.from_user.id
markup = types.ReplyKeyboardMarkup(resize_keyboard=True)
    btn1 = types.KeyboardButton("🇷🇺 Русский")
    btn2 = types.KeyboardButton('🇬🇧 English')
    markup.add(btn1, btn2)
    bot.send_message(message.from_user.id, "🇷🇺 Выберите язык / 🇬🇧 Choose your language", reply_markup=markup)

