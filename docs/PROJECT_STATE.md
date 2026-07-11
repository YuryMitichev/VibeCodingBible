# Project State

Version: 0.2.1
Status: Foundation
Last updated: 2026-07-11

---

## Текущая фаза

**Foundation (0.2.1)** — подготовка инфраструктуры для долгосрочной разработки книги.

Завершён Bootstrap (0.1.0) и инициализация **Vibe Publishing Framework** (ECR-0000). Создана система задач, логирования, архитектурная документация и первый ADR.

---

## Что готово

### Управляющие документы

| Документ | Статус | Версия |
|---|---|---|
| PROJECT_MANIFEST.md | Approved | 0.2.0 |
| ARCHITECTURE.md | Active | 0.2.1 |
| AI_CONTEXT.md | Approved | 0.2.0 |
| BOOK_OUTLINE.md | Active | 0.2.0 |
| STYLE_GUIDE.md | Approved | 0.2.0 |
| EDITOR_GUIDE.md | Active | 0.2.0 |
| ROADMAP.md | Active | 0.2.0 |
| TERMINOLOGY.md | Active | 0.2.0 |
| CHANGELOG.md | Active | 0.2.1 |
| README.md | Active | 0.2.1 |

### Vibe Publishing Framework

| Компонент | Статус |
|---|---|
| framework/ (prompts, templates, rules, workflows, schemas, checklists) | Active |
| framework/templates/ECR_TEMPLATE.md | Active |
| framework/workflows/ecr-lifecycle.md | Active |
| tasks/ (backlog, active, done) | Active |
| logs/completed/ | Active |
| ECR-0000 (initialize framework) | Done |

### ADR

| ADR | Название | Статус |
|---|---|---|
| ADR-0001 | Use Markdown and Git as Foundation | Accepted |

### Инфраструктура

- Структура каталогов репозитория (book, docs, framework, tasks, logs, templates, prompts)
- Шаблоны: chapter (полный), PRD, ADR, RFC, checklist, ECR
- Промпты: MASTER_PROMPT, bootstrap
- CI: `.github/workflows/build.yml`
- Скрипт сборки: `scripts/build.sh` (placeholder)
- Зарезервированные каталоги: playbooks, patterns, examples, diagrams

### Книга

| Раздел | Файл | Статус |
|---|---|---|
| Предисловие | book/00-FrontMatter/00-Preface.md | Stub |
| Часть I, Глава 1 | book/01-Part-I/01-What-is-Vibe-Coding.md | Stub |

---

## Что в работе

- Наполнение GLOSSARY.md и BIBLIOGRAPHY.md
- Первые черновики глав Части I
- Наполнение framework/workflows/ (workflow ревью глав, релиз)

---

## Следующие шаги

1. **0.3.0 — Outline** — финализация структуры, нумерация всех глав, карта зависимостей.
2. **0.5.0 — First Draft** — черновики всех глав.
3. **0.8.0 — Technical Review** — редактура и техническая проверка.
4. **1.0.0 — First Public Release** — публикация.

Подробнее: [ROADMAP.md](ROADMAP.md)

---

## Метрики

| Метрика | Значение |
|---|---|
| Частей книги | 10 |
| Глав (план) | 80 + приложения |
| Глав (написано) | 0 |
| Глав (черновик) | 2 (stub) |
| Шаблонов | 6 (chapter, PRD, ADR, RFC, checklist, ECR) |
| Управляющих документов | 11 |
| ADR | 1 |
| ECR (завершено) | 1 (ECR-0000) |

---

## Зарезервированные каталоги

Следующие каталоги созданы с README, наполнение — по мере необходимости:

- `playbooks/`
- `patterns/`
- `examples/`
- `diagrams/`

---

## Известные ограничения

- Сборка (PDF, EPUB, DOCX) — placeholder, не реализована.
- GLOSSARY.md и BIBLIOGRAPHY.md — заглушки.
- Workflow ревью глав и релиза — не описаны (только ECR lifecycle).

---

## Правила обновления этого документа

Обновляйте PROJECT_STATE.md после каждого логически завершённого этапа работы:

- смена фазы или версии;
- добавление или завершение глав;
- изменение структуры репозитория;
- закрытие известных ограничений;
- завершение ECR.
