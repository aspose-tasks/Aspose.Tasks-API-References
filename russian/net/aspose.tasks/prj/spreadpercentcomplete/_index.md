---
title: "Prj.SpreadPercentComplete"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, распространяется ли процент выполнения на дату статуса"
type: docs
weight: 670
url: /ru/net/aspose.tasks/prj/spreadpercentcomplete/
---
## Prj.SpreadPercentComplete field

Определяет, распределяется ли процент выполнения по дате статуса.

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadPercentComplete;
```

## Примеры

Показывает, как читать/записывать свойство Prj.SpreadPercentComplete.

```csharp
var project = new Project();

project.Set(Prj.SpreadPercentComplete, true);

Console.WriteLine("Spread Percent Complete: " + project.Get(Prj.SpreadPercentComplete));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


