---
title: "Перечисление RateFormatType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.RateFormatType. Указывает единицы, используемые Microsoft Project для отображения ставки"
type: docs
weight: 1640
url: /ru/net/aspose.tasks/rateformattype/
---
## RateFormatType enumeration

Указывает единицы измерения, используемые Microsoft Project для отображения ставки.

```csharp
public enum RateFormatType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `-1` | Значение не было определено в оригинальном файле проекта. |
| Minute | `0` | Минута (\"min\") |
| Hour | `1` | Час (\"hr\") |
| Day | `2` | День (\"day\") |
| Week | `3` | Неделя (\"wk\") |
| Month | `4` | Месяц (\"mo\") |
| Year | `5` | Год (\"yr\") |
| MaterialResourceRate | `6` | Ставка материального ресурса (пусто) |

## Примечания

При экспорте в XML неопределённые значения будут удалены из результирующего XML.

## Примеры

Показывает, как читать/записывать свойство Rsc.StandardRateFormat.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


