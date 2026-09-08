---
title: "Перечисление DayLabelDisplay"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.DayLabelDisplay. Указывает, как отображается метка дня."
type: docs
weight: 440
url: /ru/net/aspose.tasks/daylabeldisplay/
---
## DayLabelDisplay enumeration

Указывает, как отображается метка дня.

```csharp
public enum DayLabelDisplay
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| D | `0` | Устанавливает список дней в MS Project как d. |
| Dy | `1` | Устанавливает список дней в MS Project как dy. |
| Day | `2` | Устанавливает список дней в MS Project как day. |

## Примеры

Показывает, как задать метку дня в параметрах отображения проекта (случай 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// задать способ отображения метки дня
project.DisplayOptions.DayLabel = DayLabelDisplay.D;

// ...
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


