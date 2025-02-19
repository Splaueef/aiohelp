# AioHelp

AioHelp — це допоміжна бібліотека для роботи з [Aiogram](https://docs.aiogram.dev/), яка спрощує створення та налаштування Telegram-ботів.

## Основні можливості

- **Швидкий старт**: Бібліотека надає шаблони для запуску бота за кілька кроків.
- **Роутери та хендлери**: Простий спосіб обробки команд.
- **Генерація клавіатур**: Інструменти для створення клавіатур Telegram.
- **Middleware**: Легке налаштування проміжного програмного забезпечення.

## Встановлення

1. Установіть бібліотеку за допомогою `pip`:
   ```bash
   pip install aiohelp
   ```

2. Створіть структуру проекту:
   ```bash
   python -m aiohelp_project.create
   ```

## Використання

### Файл `config.py`

Додайте ваш токен у файл `config.py`:
```python
BOT_TOKEN = "your_telegram_bot_token"
```

### Хендлери

Бібліотека підтримує сучасний підхід **Aiogram 3.x**. У `handlers.py` додавайте обробку команд:
```python
from aiogram import Router, types
from aiogram.filters import Command

router = Router()

@router.message(Command(commands=["start"]))
async def start_command(message: types.Message):
    await message.answer("Привіт! Це твій бот.")
```

---

## Додаткові можливості

### Генерація клавіатур
```python
from aiohelp.keyboards import generate_keyboard

keyboard = generate_keyboard([
    ["Кнопка 1", "Кнопка 2"],
    ["Кнопка 3"]
])
```

### Middleware
```python
from aiohelp.middlewares import SimpleLoggingMiddleware

middleware = SimpleLoggingMiddleware()
```

---

## Підтримка

Якщо у вас є питання чи пропозиції, звертайтеся:
- Telegram: [Група підтримки](https://t.me/+be4T9FkKBeczMzUy)

#   a i o h e l p 
 
 #   a i o h e l p 
 
 
