# 5G NR Throughput Calculator — руководство пользователя (RU)

Этот репозиторий содержит русскоязычное руководство по эксплуатации онлайн-калькулятора пропускной способности **5G NR Throughput Calculator**.

Основной сценарий: открыть готовую HTML-версию в браузере и читать как обычную веб-страницу.

---

## Содержимое репозитория

- `calculator-user-guide.adoc` — **исходник** руководства на языке разметки AsciiDoc.
- `calculator-user-guide.html` — **готовая HTML-версия** руководства (основной файл для просмотра в браузере).
- `questions.md` — список вопросов по калькулятору (реализация, параметры, допущения).
- `images/` — изображения, используемые в статье (скриншоты интерфейса).
- `custom-style/` — кастомные CSS-стили для HTML-рендеринга руководства:
    - `custom-style/admonitions/` — стили оформления admonitions-блоков (`NOTE`, `TIP`, `WARNING` и т.д.).
    - `custom-style/user-guide/` — общие стили страницы руководства (заголовки, TOC, отступы, типографика и т.д).

Стили из `custom-style/` подключаются в `calculator-user-guide.adoc` через `include::...[]`
(например, через вставку CSS в HTML passthrough-блок `++++ ... ++++`).

Рекомендуемая структура:

```text
├─ calculator-user-guide.adoc
├─ calculator-user-guide.html
├─ questions.md
├─ images/
│  ├─ image-calc-int-1.png
│  ├─ image-calc-int-2.png
│  ├─ image-calc-int-3.png
│  └─ image-calc-int-4.png
└─ custom-style/
   ├─ admonitions/
   │  └─ admonitions.css
   └─ user-guide/
      └─ user-guide.css
```