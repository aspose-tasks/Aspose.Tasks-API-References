---
title: "Перечисление EarnedValueMethodType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.EarnedValueMethodType. Указывает метод, используемый для расчёта заработанной стоимости"
type: docs
weight: 480
url: /ru/net/aspose.tasks/earnedvaluemethodtype/
---
## EarnedValueMethodType enumeration

Указывает метод, используемый для расчёта полученной стоимости.

```csharp
public enum EarnedValueMethodType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `-1` | Поле не было определено в оригинальном файле проекта. |
| PercentComplete | `0` | Процент завершения |
| PhysicalPercentComplete | `1` | Физический процент завершения |

## Примечания

При экспорте в XML неопределённые значения будут удалены из результирующего XML.

## Примеры

Показывает, как указать метод, используемый для расчёта заработанной стоимости (EarnedValueMethodType.PercentComplete).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// установить тип метода заработанной стоимости в 'PercentComplete'
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
// работать с проектом...
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


