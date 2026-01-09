# Инструкции для Claude Code — Planora

## Особенность хранилища

Это **двухъядерное** хранилище SRT с двумя связанными системами:

- **Ядро A (Target):** Целевая система — Впечатлённый человек
- **Ядро B (Product):** Наша система — Приложение

## Структура

```
content/
├── 0.Management/           # F0 — управление хранилищем
├── A.Target/               # Ядро A: Целевая система
│   ├── A1.Suprasystem/     # Среда человека
│   ├── A2.System-of-Interest/  # Впечатлённый человек
│   └── A3.Constructor/     # ORA (ивент-продукт)
├── B.Product/              # Ядро B: Наша система
│   ├── B1.Suprasystem/     # Создатель ORA
│   ├── B2.System-of-Interest/  # Приложение
│   └── B3.Constructor/     # Planora
└── X.Bridge/               # Мосты между ядрами
```

## Нумерация семейств

| Код | Ядро | Система | Роль |
|-----|------|---------|------|
| A1.1 | Target | Suprasystem | Meaning |
| A1.2 | Target | Suprasystem | Architecture |
| A1.3 | Target | Suprasystem | Operations |
| A2.1 | Target | SoI | Meaning |
| A2.2 | Target | SoI | Architecture |
| A2.3 | Target | SoI | Operations |
| A3.1 | Target | Constructor | Meaning |
| A3.2 | Target | Constructor | Architecture |
| A3.3 | Target | Constructor | Operations |
| B1.1 | Product | Suprasystem | Meaning |
| B1.2 | Product | Suprasystem | Architecture |
| B1.3 | Product | Suprasystem | Operations |
| B2.1 | Product | SoI | Meaning |
| B2.2 | Product | SoI | Architecture |
| B2.3 | Product | SoI | Operations |
| B3.1 | Product | Constructor | Meaning |
| B3.2 | Product | Constructor | Architecture |
| B3.3 | Product | Constructor | Operations |

## Определения систем

### Ядро A

| Элемент | Система | Описание |
|---------|---------|----------|
| A1 | Среда человека | Семья, сообщество, город, инфосреда |
| A2 | Впечатлённый человек | Человек с повышенной впечатлённостью |
| A3 | ORA | Мероприятие-как-продукт |

### Ядро B

| Элемент | Система | Описание |
|---------|---------|----------|
| B1 | Создатель ORA | Организатор + площадка + инструменты |
| B2 | Приложение | Платформа для ORA |
| B3 | Planora | ИТ-служба + ORA-студия |

## Связь ядер

```
A3 (ORA) использует B2 (Приложение)
```

Подробности в `content/X.Bridge/`

## Правила работы

### Определение места документа

1. О впечатлениях, участниках, мероприятиях → **A.Target**
2. О приложении, организаторах, Planora → **B.Product**
3. О связях между ними → **X.Bridge**

### Создание документа

1. Определи ядро (A или B)
2. Определи систему (1=Suprasystem, 2=SoI, 3=Constructor)
3. Определи роль (1=Meaning, 2=Architecture, 3=Operations)
4. Размести в соответствующей папке

### Пример

Документ о требованиях к Приложению:
- Ядро: B (Product)
- Система: B2 (System-of-Interest = Приложение)
- Роль: B2.1 (Meaning = требования)
- Путь: `content/B.Product/B2.System-of-Interest/B2.1.Meaning/`

## Терминология

| Термин | Значение |
|--------|----------|
| ORA | Мероприятие-как-продукт |
| Впечатлённость | Целевая характеристика человека |
| Создатель ORA | Система, создающая мероприятия |
| Цифровой контур | Роль Приложения в создателе ORA |

## Ссылки

- [README.md](README.md) — обзор проекта
- [Определения систем](content/0.Management/0.1.%20Логика%20хранилища%20и%20знаний/systems-definition.md)
- [Мосты между ядрами](content/X.Bridge/)
