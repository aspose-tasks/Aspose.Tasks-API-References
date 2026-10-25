---
title: "Перечисление CurrencySymbolPositionType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.CurrencySymbolPositionType. Указывает положение символа валюты."
type: docs
weight: 370
url: /ru/net/aspose.tasks/currencysymbolpositiontype/
---
## CurrencySymbolPositionType enumeration

Указывает положение символа валюты.

```csharp
public enum CurrencySymbolPositionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `-1` | Указывает, что неопределённое значение означает, что поле не было определено в оригинальном файле проекта. |
| Before | `0` | Указывает тип положения символа валюты «Before». |
| After | `1` | Указывает тип положения символа валюты «After». |
| BeforeWithSpace | `2` | Указывает тип положения символа валюты «BeforeWithSpace». |
| AfterWithSpace | `3` | Указывает тип положения символа валюты «AfterWithSpace». |

## Примечания

При экспорте в XML неопределённые значения будут удалены из результирующего XML.

## Примеры

Показывает, как указать размещение символа валюты (CurrencySymbolPositionType.Before).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// установить размещение символа валюты
// Before, без пробела ($0).
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.Before);
// работать с проектом...
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


