# BKP Telegram Bot

## طريقة التشغيل

1. افتح المشروع في VS Code.
2. غيّر اسم الملف `.env.example` إلى `.env`.
3. ضع Telegram bot token و OpenAI API key داخل `.env`.
4. افتح Terminal واكتب:

```bash
pip install -r requirements.txt
python bot.py
```

## شكل ملف .env

```env
TELEGRAM_BOT_TOKEN=ضع_توكن_تيليغرام_هنا
OPENAI_API_KEY=ضع_OpenAI_API_Key_هنا
```

## اختبار البوت

افتح Telegram واكتب للبوت:

```text
/start
```

ثم اسأله:

```text
Какая цель моей ВКР?
```
