---
title: "Prj.ExtendedCreationDate"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Prj field. Дата, используемая для расчётов и отчётности"
type: docs
weight: 320
url: /ru/net/aspose.tasks/prj/extendedcreationdate/
---
## Prj.ExtendedCreationDate field

Дата, используемая для расчётов и отчётности.

```csharp
public static readonly Key<DateTime, PrjKey> ExtendedCreationDate;
```

## Примеры

Показывает, как читать/записывать свойство Prj.ExtendedCreationDate.

```csharp
var project = new Project();

project.Set(Prj.ExtendedCreationDate, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Extended Creation Date: " + project.Get(Prj.ExtendedCreationDate));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


