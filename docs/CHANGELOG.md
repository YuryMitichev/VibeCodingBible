# Changelog

Все значимые изменения проекта документируются в этом файле.

Формат основан на [Keep a Changelog](https://keepachangelog.com/ru/1.1.0/).
Версионирование следует [Semantic Versioning](https://semver.org/lang/ru/).

---

## [Unreleased]

---

## [0.2.1] — 2026-07-11

### Added

- **Vibe Publishing Framework** — каталог `framework/` с prompts, templates, rules, workflows, schemas, checklists
- Система задач `tasks/` (backlog, active, done) и логирование `logs/completed/`
- Шаблон ECR: `framework/templates/ECR_TEMPLATE.md`
- Workflow жизненного цикла ECR: `framework/workflows/ecr-lifecycle.md`
- Архитектурная документация: `docs/ARCHITECTURE.md`
- ADR-каталог `docs/adr/` и [ADR-0001: Use Markdown and Git as Foundation](adr/ADR-0001-use-markdown.md)
- Зарезервированные каталоги с README: `playbooks/`, `patterns/`, `examples/`, `diagrams/`
- ECR-0000: `tasks/done/ECR-0000-initialize-framework.md`
- Отчёт ECR-0000: `logs/completed/ECR-0000-report.md`

### Changed

- README.md — полная структура репозитория, раздел ECR, ссылка на ARCHITECTURE
- templates/chapter.template.md — полноценный шаблон главы (10 разделов)
- tasks/README.md — синхронизация с lifecycle Backlog → Planned → Active → Review → Done → Archived
- docs/PROJECT_STATE.md — версия 0.2.1, статус инфраструктуры фреймворка

---

## [0.2.0] — 2026-07-11

### Added

- README.md — точка входа в проект с навигацией и быстрым стартом
- docs/EDITOR_GUIDE.md — рабочий процесс для авторов и редакторов
- docs/ROADMAP.md — дорожная карта от Foundation до 1.0.0
- docs/TERMINOLOGY.md — единый словарь терминов проекта

### Changed

- docs/PROJECT_STATE.md — обновлён до фазы Foundation (0.2.0)
- docs/AI_CONTEXT.md — исправлен дублирующийся фрагмент в конце документа

### Existing (без изменений содержания)

- docs/PROJECT_MANIFEST.md — v0.2.0, Approved
- docs/BOOK_OUTLINE.md — v0.2.0, Active
- docs/STYLE_GUIDE.md — v0.2.0, Approved

---

## [0.1.0] — 2026

### Added

- Bootstrap: структура репозитория (book/, docs/, templates/, prompts/, scripts/, build/)
- Заглушки управляющих документов
- Заглушки глав: Preface, Chapter 1
- Шаблоны: chapter, PRD, ADR, RFC, checklist
- Промпты: MASTER_PROMPT, bootstrap
- CI: GitHub Actions workflow
- LICENSE

[Unreleased]: https://github.com/compare/v0.2.1...HEAD
[0.2.1]: https://github.com/compare/v0.2.0...v0.2.1
[0.2.0]: https://github.com/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/compare/initial...v0.1.0

## [0.2.2] - 2026-07-12

### Added
- Полный текст Главы 1: "Последний инструмент, который вам придётся изучить"
- Файл-заглушка для Главы 2: "Что такое Vibe Coding"

### Changed
- Обновлён BOOK_OUTLINE.md (добавлена Глава 1, все главы сдвинуты на +1)
- Обновлён PROJECT_STATE.md (статусы глав)
- Переименован файл: 01-What-is-Vibe-Coding.md → 01-The-Last-Tool.md

## [0.2.3] - 2026-07-12

## [0.2.3] - 2026-07-12

### Added
- Полный текст Главы 2: "Что такое Vibe Coding"

### Changed
- Обновлён PROJECT_STATE.md (статус главы 2: финальная)
- Обновлён BOOK_OUTLINE.md (глава 2 отмечена как завершённая)

## [0.2.4] - 2026-07-12

### Added
- Полный текст Главы 3: "Как изменился процесс разработки"

### Changed
- Переписана Глава 2: "Что такое Vibe Coding" (адаптирована для новичков)
- Обновлён BOOK_OUTLINE.md (глава 3 отмечена как завершённая, обновлено описание)
- Обновлён PROJECT_STATE.md (статус глав 2 и 3: финальные)