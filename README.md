# AI-агент продаж e-KNOT (онлайн-голосование)

Воронка: анализ чата → лид → портрет клиента → холодный контакт → продажа.

## Қосу
```
pip install -r requirements.txt
cp .env.example .env   # GEMINI_API_KEY қойыңыз (aistudio.google.com)
python funnel.py       # воронка, нәтиже results.json
python pilot.py        # пилот: чат-бот менеджер
```

## Құрылым
- `prompts.py` — барлық промпттар
- `funnel.py` — чат талдау, лид, портрет, холодный контакт
- `pilot.py` — сатушы-бот диалогы (пилот)
- `data/chats.json` — тест чаттар (3 мысал: 2 лид, 1 лид емес)

## Келесі қадам
Google Cloud серверіне орналастыру, содан кейін WhatsApp (Cloud API) қосу.
