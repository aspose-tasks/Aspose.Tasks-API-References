---
title: "Prj.StartDate"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Дата начала проекта"
type: docs
weight: 680
url: /ru/net/aspose.tasks/prj/startdate/
---
## Prj.StartDate field

Дата начала проекта.

```csharp
public static readonly Key<DateTime, PrjKey> StartDate;
```

## Примеры

Показывает, как читать/записывать свойство Prj.StartDate.

```csharp
var project = new Project();

project.Set(Prj.StartDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Start Date: " + project.Get(Prj.StartDate));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


