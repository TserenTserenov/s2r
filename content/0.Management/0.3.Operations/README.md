---
system: "Management"
role: "Operations"
title: "Операции управления: процессы и практики"
date: "2026-01-07"
tags: [management, operations, processes, workflows]
status: "active"
related:
  - ../README.md
  - ../0.1.Meaning/README.md
  - ../0.2.Architecture/README.md
fpf_principles:
  - practicality
  - incremental-improvement
---

# Операции управления (0.3.Operations)

## Назначение раздела

Здесь документируются **процессы работы** с хранилищем: workflows, создание документов, интеграция с AI.

**Вопрос раздела:** Как работает?

## Содержимое раздела

| Документ | Описание |
|----------|----------|
| [workflows.md](workflows.md) | Процессы работы с хранилищем |
| [claude-fpf.md](claude-fpf.md) | Интеграция Claude Code и FPF |
| [document-creation.md](document-creation.md) | Создание документов |

## Что здесь размещается

- **Процессы** — workflows для типовых задач
- **Инструкции** — пошаговые руководства
- **Интеграции** — работа с внешними инструментами
- **Автоматизация** — CI/CD, pre-commit hooks

## Связь с FPF

Раздел реализует паттерны:
- **A.15 (Role-Method-Work Alignment)** — связь ролей, методов и работы
- **A.15.1 (U.Work)** — записи о выполненной работе

## Шаблон документа

```markdown
---
type: process
status: draft
created: YYYY-MM-DD
updated: YYYY-MM-DD
system: "Management"
role: "Operations"
related: []
fpf_principles: []
---

# Название процесса

## Назначение

[Краткое описание цели]

## Процесс

### Шаг 1: [Название]

[Описание]

### Шаг 2: [Название]

[Описание]

## Changelog

| Дата | Изменение | Автор |
|------|-----------|-------|

## Связанные документы

- [Документ](path.md)
```

## Связанные документы

- [Раздел Management](../README.md)
- [Смысл управления](../0.1.Meaning/README.md)
- [Архитектура управления](../0.2.Architecture/README.md)
