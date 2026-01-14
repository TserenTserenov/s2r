---
type: doc
status: active
created: 2026-01-14
updated: 2026-01-14
family: F0
scope: repository
---

# Соглашения об именовании (Naming Conventions)

## Общие правила

1. **Папки** — только на английском
2. **Файлы** — могут быть на русском или английском
3. **Используй kebab-case** для файлов: `my-document.md`
4. **Используй PascalCase или числовую нумерацию** для папок

## Именование папок

### Корневой уровень

```
0.OPS/     # Числовой префикс + PascalCase
A.Impressed-Customer/        # Буква ядра + имя целевой системы
B.Mobile-App/                # Буква ядра + имя нашей системы
```

### Уровень системы

> **Важно:** Используйте имена конкретных систем, а не абстрактные роли.

```
Хорошо:
A1.Daily-Life/               # Имя надсистемы
A2.Impressed-Customer/       # Имя целевой системы (SoI)
A3.Product-Ecosystem/        # Имя конструктора

Плохо:
A1.Suprasystem/              # Это роль, не имя системы
A2.System-of-Interest/       # Абстрактно
A3.Constructor/              # Не описывает, ЧТО создаёт
```

### Уровень роли

```
X1.1.Meaning/                # X = ядро, 1 = система, .1/.2/.3 = роль
X1.2.Architecture/
X1.3.Operations/
```

> Роли остаются фиксированными: Meaning, Architecture, Operations

### Уровень F0

```
0.1.Knowledge-Logic/         # Функциональная область
0.2.Repository-Processes/
0.3.Kernels-Bridge/
0.4.Plans-and-Meetings/
0.5.AI-Reports/
0.9.Inbox/
0.99.Archive/
```

## Именование файлов

### Документы

```
requirements.md              # Простое имя
api-specification.md         # kebab-case для составных
team-structure.md
value-chain.md
```

### README файлы

```
README.md                    # Всегда UPPERCASE
```

### Специальные файлы

```
local-ontology.md            # В X0.{System-Name}-Management/
_index.md                    # Если нужен индекс (редко)
```

## Паттерны именования ядер

### Хорошо

```
A.Impressed-Person/          # Конкретно, понятно
B.Mobile-App/                # Описывает систему
C.Backend-Service/           # Технически точно
D.Analytics-Platform/        # Функционально
```

### Плохо

```
A.Target/                    # Слишком абстрактно
B.System2/                   # Неинформативно
C.Module/                    # Размыто
D.Other/                     # Бессмысленно
```

## Примеры полных путей

### Хорошо (с именами систем)

```
0.OPS/0.1.Knowledge-Logic/01-kernels-model.md
A.Impressed-Customer/A2.Impressed-Customer/A2.1.Meaning/requirements.md
B.Mobile-App/B3.Dev-Team/B3.3.Operations/team-structure.md
C.Backend-Service/C2.Backend-Service/C2.2.Architecture/api-schema.md
```

### Плохо (абстрактные названия)

```
A.Target-System/A2.System-of-Interest/A2.1.Meaning/requirements.md
B.Our-System/B3.Constructor/B3.3.Operations/team-structure.md
```

## См. также

- [06-taxonomy.md](06-taxonomy.md) — классификация документов
- [../0.2.Repository-Processes/standards.md](../0.2.Repository-Processes/standards.md) — стандарты
