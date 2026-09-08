---
title: "Перечисление HourLabelDisplay"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.HourLabelDisplay перечисление. Указывает, как отображается метка часа"
type: docs
weight: 820
url: /ru/net/aspose.tasks/hourlabeldisplay/
---
## HourLabelDisplay enumeration

Указывает, как отображается метка часа.

```csharp
public enum HourLabelDisplay
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| H | `0` | \"h\" метка. |
| Hr | `1` | \"hr\" метка. |
| Hour | `2` | \"hour(s)\" метка. |

## Примеры

Показывает, как установить метку часа в параметрах отображения проекта (случай 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// установить, как отображается метка часа
project.DisplayOptions.HourLabel = HourLabelDisplay.H;

// ...
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


