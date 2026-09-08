---
title: "Перечисление YearLabelDisplay"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.YearLabelDisplay. Указывает, как отображается метка года."
type: docs
weight: 3680
url: /ru/net/aspose.tasks/yearlabeldisplay/
---
## YearLabelDisplay enumeration

Указывает, как отображается метка года.

```csharp
public enum YearLabelDisplay
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Y | `0` | Устанавливает список лет в MS Project как mo. |
| Yr | `1` | Устанавливает список лет в MS Project как mon. |
| Year | `2` | Устанавливает список лет в MS Project как месяц. |

## Примеры

Показывает, как установить метку года в параметрах отображения проекта (случай 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// установить, как отображается метка года
project.DisplayOptions.YearLabel = YearLabelDisplay.Y;

// ...
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


