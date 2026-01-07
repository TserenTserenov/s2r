---
system: "Management"
role: "Architecture"
title: "Архитектура управления: структура и роли"
date: "2026-01-07"
tags: [management, architecture, structure, roles]
status: "active"
related:
  - ../README.md
  - ../0.1.Meaning/README.md
  - ../0.3.Operations/README.md
fpf_principles:
  - systemic-thinking
  - clarity
  - srd-structure
---

# Архитектура управления (0.2.Architecture)

## Назначение раздела

Здесь документируется **структура хранилища**: организация папок, роли участников, стандарты оформления.

**Вопрос раздела:** Как устроено?

## Содержимое раздела

| Документ | Описание |
|----------|----------|
| [structure.md](structure.md) | Структура хранилища и папок |
| [roles.md](roles.md) | Роли и ответственность участников |
| [standards.md](standards.md) | Стандарты оформления документов |

## Что здесь размещается

- **Структура** — организация папок и файлов
- **Роли** — участники и их ответственность
- **Стандарты** — правила оформления
- **Схемы** — визуализации архитектуры

## Связь с FPF

Раздел реализует паттерны:
- **A.1 (Holonic Foundation)** — иерархия папок как холоны
- **A.2 (Role Taxonomy)** — классификация ролей

## Шаблон документа

```markdown
---
type: doc
status: draft
created: YYYY-MM-DD
updated: YYYY-MM-DD
system: "Management"
role: "Architecture"
related: []
fpf_principles: []
---

# Название

## Назначение документа

[Краткое описание]

## Структура

[Описание структуры]

## Компоненты

[Элементы структуры]

## Changelog

| Дата | Изменение | Автор |
|------|-----------|-------|

## Связанные документы

- [Документ](path.md)
```

## Связанные документы

- [Раздел Management](../README.md)
- [Смысл управления](../0.1.Meaning/README.md)
- [Операции управления](../0.3.Operations/README.md)
