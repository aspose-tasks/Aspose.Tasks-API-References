---
title: "Перечисление MonthLabelDisplay"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.MonthLabelDisplay. Указывает, как отображается метка месяца"
type: docs
weight: 1060
url: /ru/net/aspose.tasks/monthlabeldisplay/
---
## MonthLabelDisplay enumeration

Указывает, как отображается метка месяца.

```csharp
public enum MonthLabelDisplay
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Mo | `0` | Устанавливает список месяцев в MS Project как mo. |
| Mon | `1` | Устанавливает список месяцев в MS Project как mon. |
| Month | `2` | Устанавливает список месяцев в MS Project как month. |

## Примеры

Показывает, как установить метку месяца в параметрах отображения проекта (пример 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// установить, как отображается метка месяца
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mo;

// ...
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


