---
title: "Project.GetBaselineSaveTime"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Возвращает время сохранения базовой линии"
type: docs
weight: 1090
url: /ru/net/aspose.tasks/project/getbaselinesavetime/
---
## Project.GetBaselineSaveTime method

Возвращает время сохранения базовой линии.

```csharp
public DateTime GetBaselineSaveTime(BaselineType baselineNumber)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| baselineNumber | BaselineType | Номер базовой линии [`BaselineType`](../../baselinetype/). |

### Возвращаемое значение

Дата и время последнего сохранения базовой линии.

## Примечания

Возвращает DateTime.MinValue, если базовая линия не была сохранена.

## Примеры

Показывает, как читать/записывать время сохранения базовой линии проекта.

```csharp
var project = new Project();
var baselineSave = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time before: " + baselineSave);

// установить время сохранения базовой линии
project.SetBaselineSaveTime(BaselineType.Baseline, DateTime.Today);

var baselineSaveNew = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time after: " + baselineSaveNew);
```

### См. также

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


