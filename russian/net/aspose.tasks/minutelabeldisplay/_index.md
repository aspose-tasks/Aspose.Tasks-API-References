---
title: "Перечисление MinuteLabelDisplay"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.MinuteLabelDisplay. Указывает, как отображается метка минут."
type: docs
weight: 1030
url: /ru/net/aspose.tasks/minutelabeldisplay/
---
## MinuteLabelDisplay enumeration

Указывает, как отображается метка минуты.

```csharp
public enum MinuteLabelDisplay
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| M | `0` | Устанавливает список Minutes в MS Project как m. |
| Min | `1` | Устанавливает список Minutes в MS Project как min. |
| Minute | `2` | Устанавливает список Minutes в MS Project как minute. |

## Примеры

Показывает, как установить метку минут в параметрах отображения проекта (случай 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// устанавливает, как отображается метка минут
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.M;

// ...
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


