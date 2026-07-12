# Vibe Coding Bible

Практическое руководство по AI-assisted разработке программного обеспечения.

Репозиторий организован как **knowledge monorepo** — единый источник знаний для книги, курса, документации и шаблонов. Процессы разработки и изменений описаны в **Vibe Publishing Framework** (`framework/`).

---

## Статус проекта

| Параметр | Значение |
|---|---|
| Версия | 0.2.1 |
| Фаза | Foundation |
| Статус | Active |

Подробнее: [docs/PROJECT_STATE.md](docs/PROJECT_STATE.md)

---

## Для кого этот проект

- разработчики, которые хотят выстроить процесс работы с ИИ;
- технические лидеры и архитекторы;
- авторы и редакторы, участвующие в написании книги;
- ИИ-инструменты, которым нужен постоянный контекст проекта.

---

## Быстрый старт

### Для участников проекта

1. Ознакомьтесь с [docs/PROJECT_MANIFEST.md](docs/PROJECT_MANIFEST.md) — миссия, принципы, структура.
2. Прочитайте [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md) — архитектура репозитория и роли каталогов.
3. Изучите [docs/AI_CONTEXT.md](docs/AI_CONTEXT.md) — философия, тон, правила работы с ИИ.
4. Ознакомьтесь с [docs/BOOK_OUTLINE.md](docs/BOOK_OUTLINE.md) — структура книги из 10 частей.
5. Следуйте [docs/STYLE_GUIDE.md](docs/STYLE_GUIDE.md) и [docs/EDITOR_GUIDE.md](docs/EDITOR_GUIDE.md) при написании материалов.

### Для ИИ-инструментов

Перед началом работы изучите:

- [docs/PROJECT_STATE.md](docs/PROJECT_STATE.md)
- [docs/PROJECT_MANIFEST.md](docs/PROJECT_MANIFEST.md)
- [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md)
- [docs/AI_CONTEXT.md](docs/AI_CONTEXT.md)
- [docs/BOOK_OUTLINE.md](docs/BOOK_OUTLINE.md)
- [docs/STYLE_GUIDE.md](docs/STYLE_GUIDE.md)

Постоянный промпт: [prompts/MASTER_PROMPT.md](prompts/MASTER_PROMPT.md)

---

## Структура репозитория

```
VibeCodingBible/
├── book/              # Текст книги (главы по частям)
├── docs/              # Управляющие документы и ADR
│   └── adr/           # Architecture Decision Records
├── framework/         # Vibe Publishing Framework (процессы, шаблоны ECR)
│   ├── prompts/       # Универсальные промпты фреймворка
│   ├── templates/     # Шаблоны ECR и служебных документов
│   ├── rules/         # Правила и конвенции
│   ├── workflows/     # Рабочие процессы (ECR, ревью, релиз)
│   ├── schemas/       # Схемы и форматы данных
│   └── checklists/    # Чек-листы фреймворка
├── tasks/             # Задачи ECR (backlog → active → done)
├── logs/              # Отчёты о завершённых ECR
│   └── completed/     # Архив отчётов
├── templates/         # Шаблоны глав, PRD, ADR, RFC, чек-листов
├── prompts/           # Промпты для ИИ (контекст книги)
├── playbooks/         # Практические сценарии
├── patterns/          # Паттерны и повторяемые решения
├── examples/          # Примеры и эталонные фрагменты
├── diagrams/          # Диаграммы и визуальные материалы
├── checklists/        # Готовые чек-листы проекта
├── scripts/           # Скрипты сборки
├── build/             # Инструкции и артефакты сборки
├── .cursor/           # Конфигурация Cursor IDE
└── .github/           # CI/CD
```

---

## Ключевые документы

| Документ | Назначение |
|---|---|
| [PROJECT_MANIFEST.md](docs/PROJECT_MANIFEST.md) | Миссия, принципы, стандарты качества |
| [ARCHITECTURE.md](docs/ARCHITECTURE.md) | Архитектура репозитория |
| [PROJECT_STATE.md](docs/PROJECT_STATE.md) | Текущее состояние проекта |
| [AI_CONTEXT.md](docs/AI_CONTEXT.md) | Контекст для ИИ-инструментов |
| [BOOK_OUTLINE.md](docs/BOOK_OUTLINE.md) | Структура и план книги |
| [STYLE_GUIDE.md](docs/STYLE_GUIDE.md) | Стиль и формат глав |
| [EDITOR_GUIDE.md](docs/EDITOR_GUIDE.md) | Руководство для редакторов |
| [ROADMAP.md](docs/ROADMAP.md) | Дорожная карта разработки |
| [TERMINOLOGY.md](docs/TERMINOLOGY.md) | Единая терминология |
| [CHANGELOG.md](docs/CHANGELOG.md) | История изменений |
| [GLOSSARY.md](docs/GLOSSARY.md) | Глоссарий (для читателей) |
| [BIBLIOGRAPHY.md](docs/BIBLIOGRAPHY.md) | Рекомендуемая литература |

---

## Задачи и изменения (ECR)

Изменения в репозитории оформляются как **Engineering Change Request** (ECR-XXXX):

- шаблон: [framework/templates/ECR_TEMPLATE.md](framework/templates/ECR_TEMPLATE.md)
- жизненный цикл: [framework/workflows/ecr-lifecycle.md](framework/workflows/ecr-lifecycle.md)
- задачи: [tasks/](tasks/)
- отчёты: [logs/completed/](logs/completed/)

---

## Написание глав

1. Выберите главу из [BOOK_OUTLINE.md](docs/BOOK_OUTLINE.md).
2. Создайте или откройте файл в `book/` по соглашению: `NN-Part-X/NN-Chapter-Title.md`.
3. Используйте шаблон: [templates/chapter.template.md](templates/chapter.template.md).
4. Соблюдайте [STYLE_GUIDE.md](docs/STYLE_GUIDE.md) и [TERMINOLOGY.md](docs/TERMINOLOGY.md).
5. Добавьте ссылки на связанные главы.

---

## Принципы проекта

- **Практика важнее теории** — каждая концепция сопровождается примером.
- **Независимость от инструментов** — принципы, а не инструкции к одному сервису.
- **ИИ усиливает инженера** — ответственность всегда остаётся за человеком.
- **Эволюционность** — материал обновляется без полной переработки.

---

## Лицензия

См. [LICENSE](LICENSE).
