# Tasks

Система задач Vibe Publishing Framework.

## Жизненный цикл задачи

```
Backlog → Planned → Active → Review → Done → Archived
```

Полное описание стадий, критериев и переходов: [framework/workflows/ecr-lifecycle.md](../framework/workflows/ecr-lifecycle.md).

| Стадия | Описание |
|---|---|
| **Backlog** | Идея зафиксирована, работа не спланирована |
| **Planned** | Объём и критерии готовности определены |
| **Active** | Реализация в процессе |
| **Review** | Изменения готовы к проверке |
| **Done** | ECR принят, отчёт создан |
| **Archived** | Историческая запись, активная работа не ведётся |

---

## Соответствие каталогам

Физические каталоги отражают **группы стадий**, а не каждую стадию отдельно:

| Каталог | Стадии | Описание |
|---|---|---|
| [backlog/](backlog/) | Backlog, Planned | Очередь и запланированные задачи |
| [active/](active/) | Active, Review | Задачи в работе или на ревью |
| [done/](done/) | Done, Archived | Завершённые и архивные задачи |

**Статус Planned или Review** указывается в front matter или заголовке файла ECR, пока файл находится в соответствующем каталоге.

---

## Формат идентификатора

Каждая задача имеет идентификатор **ECR-XXXX**:

```
ECR-0000
ECR-0001
ECR-0002
```

- **ECR** — Engineering Change Request
- **XXXX** — четырёхзначный порядковый номер с ведущими нулями

---

## Файл задачи

Задача оформляется по шаблону [framework/templates/ECR_TEMPLATE.md](../framework/templates/ECR_TEMPLATE.md).

Рекомендуемое имя файла: `ECR-XXXX-short-title.md`

Рекомендуемый front matter (опционально):

```markdown
**Статус:** Backlog | Planned | Active | Review | Done | Archived
**Дата создания:** YYYY-MM-DD
**Дата завершения:** YYYY-MM-DD
```

---

## Переходы между стадиями

| Переход | Действие |
|---|---|
| Backlog → Planned | Заполнены «Изменения» и «Критерии готовности» |
| Planned → Active | Файл перемещён в `active/`, начата реализация |
| Active → Review | Реализация завершена, выполнена самопроверка |
| Review → Active | Замечания ревью, доработка |
| Review → Done | Критерии готовности выполнены, ECR принят |
| Done → Archived | ECR включён в историю проекта, правки не вносятся |

При переходе в **Done**:

1. Файл перемещается в `done/`
2. Создаётся отчёт в [logs/completed/](../logs/completed/) — см. [logs/README.md](../logs/README.md)
3. При значимых изменениях обновляются [CHANGELOG.md](../docs/CHANGELOG.md) и [PROJECT_STATE.md](../docs/PROJECT_STATE.md)

---

## Пример: ECR-0000

Первый завершённый ECR — инициализация фреймворка:

- Задача: [done/ECR-0000-initialize-framework.md](done/ECR-0000-initialize-framework.md)
- Отчёт: [logs/completed/ECR-0000-report.md](../logs/completed/ECR-0000-report.md)

---

## Связанные документы

- [framework/workflows/ecr-lifecycle.md](../framework/workflows/ecr-lifecycle.md)
- [framework/templates/ECR_TEMPLATE.md](../framework/templates/ECR_TEMPLATE.md)
- [logs/README.md](../logs/README.md)
- [docs/ARCHITECTURE.md](../docs/ARCHITECTURE.md)
