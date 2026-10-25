---
title: "Перечисление BaselineType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.BaselineType. Указывает тип базовой линии, используемый для расчёта значений отклонения"
type: docs
weight: 130
url: /ru/net/aspose.tasks/baselinetype/
---
## BaselineType enumeration

Указывает тип базовой линии, используемый для расчёта значений отклонения.

```csharp
public enum BaselineType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `-1` | Указывает, что поле не было определено в оригинальном файле проекта. |
| Baseline | `0` | Указывает тип базовой линии. |
| Baseline1 | `1` | Указывает тип Baseline1. |
| Baseline2 | `2` | Указывает тип Baseline2. |
| Baseline3 | `3` | Указывает тип Baseline3. |
| Baseline4 | `4` | Указывает тип Baseline4. |
| Baseline5 | `5` | Указывает тип Baseline5. |
| Baseline6 | `6` | Указывает тип Baseline6. |
| Baseline7 | `7` | Указывает тип Baseline7. |
| Baseline8 | `8` | Указывает тип Baseline8. |
| Baseline9 | `9` | Указывает тип Baseline9. |
| Baseline10 | `10` | Указывает тип Baseline10. |

## Примечания

При экспорте в XML неопределённые значения будут удалены из результирующего XML.

## Примеры

Показывает, как установить базовую линию для проекта (BaselineType.Baseline).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// Сохранить поля базовой линии в указанную базовую линию для всего проекта.
project.SetBaseline(BaselineType.Baseline);
// Работа с базовыми линиями проекта...
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


