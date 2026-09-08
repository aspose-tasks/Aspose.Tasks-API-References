---
title: "Prj.CurrentDate"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Системная дата"
type: docs
weight: 190
url: /ru/net/aspose.tasks/prj/currentdate/
---
## Prj.CurrentDate field

Системная дата.

```csharp
public static readonly Key<DateTime, PrjKey> CurrentDate;
```

## Примеры

Показывает, как читать/записывать свойство Prj.CurrentDate.

```csharp
var project = new Project();

project.Set(Prj.CurrentDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Current Date: " + project.Get(Prj.CurrentDate));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


