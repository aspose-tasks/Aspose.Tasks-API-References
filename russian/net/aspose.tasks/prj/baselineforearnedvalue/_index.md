---
title: "Prj.BaselineForEarnedValue"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Prj field. Конкретная базовая линия, используемая для расчёта значений отклонения"
type: docs
weight: 80
url: /ru/net/aspose.tasks/prj/baselineforearnedvalue/
---
## Prj.BaselineForEarnedValue field

Конкретная базовая линия, используемая для расчёта значений отклонения.

```csharp
public static readonly Key<BaselineType, PrjKey> BaselineForEarnedValue;
```

## Примеры

Показывает, как читать/записывать свойство Prj.BaselineForEarnedValue.

```csharp
var project = new Project();

project.Set(Prj.BaselineForEarnedValue, BaselineType.Baseline);

Console.WriteLine("Baseline For Earned Value: " + project.Get(Prj.BaselineForEarnedValue));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BaselineType](../../baselinetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


