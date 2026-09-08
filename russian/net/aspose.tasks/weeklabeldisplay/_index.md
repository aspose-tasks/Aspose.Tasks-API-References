---
title: "Перечисление WeekLabelDisplay"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.WeekLabelDisplay. Указывает, как отображается метка недели."
type: docs
weight: 3560
url: /ru/net/aspose.tasks/weeklabeldisplay/
---
## WeekLabelDisplay enumeration

Указывает, как отображается метка недели.

```csharp
public enum WeekLabelDisplay
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| W | `0` | "w" метка. |
| Wk | `1` | "wk" метка. |
| Week | `2` | "week" метка. |

## Примеры

Показывает, как задать метку недели в параметрах отображения проекта (случай 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// задать способ отображения метки недели
project.DisplayOptions.WeekLabel = WeekLabelDisplay.W;

// ...
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


