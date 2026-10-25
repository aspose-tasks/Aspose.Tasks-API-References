---
title: "Prj.EarnedValueMethod"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Метод расчёта заработанной стоимости по умолчанию"
type: docs
weight: 310
url: /ru/net/aspose.tasks/prj/earnedvaluemethod/
---
## Prj.EarnedValueMethod field

Метод расчёта заработанной стоимости по умолчанию.

```csharp
public static readonly Key<EarnedValueMethodType, PrjKey> EarnedValueMethod;
```

## Примеры

Показывает, как читать/записывать свойство Prj.EarnedValueMethod.

```csharp
var project = new Project();

project.Set(Prj.EarnedValueMethod, EarnedValueMethodType.PhysicalPercentComplete);

Console.WriteLine("Earned Value Method: " + project.Get(Prj.EarnedValueMethod));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


