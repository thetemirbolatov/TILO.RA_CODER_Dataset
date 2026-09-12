# TILO.RA CODER Dataset

Объединённый русско-английский датасет для обучения и поиска по коду.
Формат — пары `question` / `code`: вопрос на естественном языке → готовый код-ответ.

Датасет собран для локального ассистента **TILO.RA CODER** — офлайн-помощника по программированию

# Скачать по ссылке 

https://github.com/thetemirbolatov/TILO.RA_CODER_Dataset/releases/download/v1.0.0/tilora_knowledge_merged.jsonl


## Состав

| Источник | Язык | Записей |
|---|---|---|
| English coding dialogs | en | ~156 000 |
| Russian code Q&A | ru | ~143 000 |
| **Итого** | **ru + en** | **~299 000** |

После удаления дубликатов и пустых записей остаётся около **180 000 – 300 000** пар (зависит от версии сборки).

## Формат

Каждая строка — JSON-объект:

```json
{
  "question": "Как отсортировать словарь по значению?",
  "code": "sorted_dict = dict(sorted(d.items(), key=lambda x: x[1]))"
}
