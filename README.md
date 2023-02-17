# VK Lab NLP 

Исследуется задача сегментации текстов. Её суть заключается в разбиении текста на части, состоящих из близких по смыслу и теме предложений.
В качестве решения задачи предлагается использовать композицию из двух biLSTM моделей.

В файле data.jsonl содержится набор текстов историй с сайта tjournal.ru, разбитых на предложения. В каждой отдельной строке содержится массив пар (предложение, класс), где классы: 1 — первое предложение абзаца, 2 — первое предложение секции, 0 — остальные предложения (части абзацев).

Реализуется решение, позволяющее:

Автоматически разбивать текст на абазцы
Автоматически разбивать текст на секции

Для теста используются f1, accuracy, precision, recall метрики.
