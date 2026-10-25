---
title: "Класс Rate"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Rate. Представляет определение временного периода и ставок, применимых к ресурсу в течение этого периода"
type: docs
weight: 1610
url: /ru/net/aspose.tasks/rate/
---
## Rate class

Представляет определение временного периода и ставок, применимых к ресурсу в течение этого периода.

```csharp
public class Rate
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CostPerUse](../../aspose.tasks/rate/costperuse/) { get; set; } | Получает или задает стоимость использования ресурса. Это значение извлекается из текущей даты, если для ресурса существует таблица ставок. |
| [OvertimeRate](../../aspose.tasks/rate/overtimerate/) { get; set; } | Получает или задает ставку сверхурочных за час для ресурса. |
| [OvertimeRateFormat](../../aspose.tasks/rate/overtimerateformat/) { get; set; } | Получает или задает единицы, используемые Microsoft Project для отображения ставки сверхурочных. |
| [RatesFrom](../../aspose.tasks/rate/ratesfrom/) { get; set; } | Получает или задает дату вступления ставки в силу. |
| [RatesTo](../../aspose.tasks/rate/ratesto/) { get; set; } | Получает или задает последнюю дату, когда ставка действует. |
| [RateTable](../../aspose.tasks/rate/ratetable/) { get; set; } | Получает или задает уникальный идентификатор таблицы ставок для ресурса. |
| [StandardRate](../../aspose.tasks/rate/standardrate/) { get; set; } | Получает или задает стандартную ставку за час для ресурса. |
| [StandardRateFormat](../../aspose.tasks/rate/standardrateformat/) { get; set; } | Получает или задает единицы, используемые Microsoft Project для отображения стандартной ставки. |

## Примеры

Показывает, как работать со ставками ресурсов.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RateTable = RateType.A;
rate1.RatesFrom = new DateTime(2019, 1, 1, 8, 0, 0);
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;
rate1.OvertimeRate = 10m;
rate1.OvertimeRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0));
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;
rate2.CostPerUse = 2m;

// работать с проектом...
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


