                                                               My_bot
Телеграм-бот создан для конвертации валют. Имя в телеграме  @Valuta_bot.
В Telegram-боте реализован следующий функционал:
1.	Бот возвращает цену на определённое количество валюты (евро, доллар или рубль).
2.	При написании бота использована библиотека pytelegrambotapi.
3.	Человек должен отправить сообщение боту в виде <имя валюты> <в какую валюту надо перевести> <количество переводимой валюты>.
4.	При вводе команды /start или /help пользователю выводятся инструкции по применению бота.
5.	При вводе команды /values  выводится информация о всех доступных валютах в читаемом виде.
6.	Для взятия курса валют использовано API, взятое из сайта https://www.cryptocompare.com/ и отправлены к нему запросы с помощью библиотеки Requests.
7.	Для парсинга полученных ответов использована библиотека JSON.
8.	При ошибке пользователя (например, введена неправильная или несуществующая валюта или неправильно введено число) выводится собственно написанное исключение APIException с текстом пояснения ошибки.
9.	Текст любой ошибки с указанием типа ошибки отправляется пользователю в сообщения.
10.	Для отправки запросов к  API описан класс со статическим методом get_price(), который принимает три аргумента: имя валюты, цену на которую надо узнать, — base, имя валюты, цену в которой надо узнать, — quote, количество переводимой валюты — amount и возвращает нужную сумму в валюте.
11.	Токен telegramm-бота хранится в специальном конфиге.
12.	Все классы спрятаны в файле extensions.py.

Данный бот не запущен, необходимо запустить бот со своего устройства (загрузить данный репозиторий на свой компьютер) Для работы с данным телеграм-ботом необходимо установить пакеты requests и PyTelegramBotAPI (версия 4.X).


