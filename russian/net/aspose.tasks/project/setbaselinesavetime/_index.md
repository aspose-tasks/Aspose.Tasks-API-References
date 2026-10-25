---
title: "Project.SetBaselineSaveTime"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Устанавливает время сохранения базовой линии."
type: docs
weight: 1260
url: /ru/net/aspose.tasks/project/setbaselinesavetime/
---
## Project.SetBaselineSaveTime method

Устанавливает время сохранения базового плана.

```csharp
public void SetBaselineSaveTime(BaselineType baselineNumber, DateTime value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| baselineNumber | BaselineType | Номер базовой линии [`BaselineType`](../../baselinetype/). |
| value | DateTime | Дата и время последнего сохранения базовой линии. |

## Примечания

Установите значение DateTime.MinValue, если базовая линия не была сохранена.

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


