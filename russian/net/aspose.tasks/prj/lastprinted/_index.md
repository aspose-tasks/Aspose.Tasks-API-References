---
title: "Prj.LastPrinted"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Время последней печати проекта. Сохраняется в формате UTC в файлах mpp. Тип DateTime."
type: docs
weight: 430
url: /ru/net/aspose.tasks/prj/lastprinted/
---
## Prj.LastPrinted field

Время последней печати проекта. Сохранено в формате UTC в файлах mpp. Тип DateTime.

```csharp
public static readonly Key<DateTime, PrjKey> LastPrinted;
```

## Примеры

Показывает, как читать/записывать свойство Prj.LastPrinted.

```csharp
var project = new Project();

project.Set(Prj.LastPrinted, new DateTime(2020, 4, 10, 13, 0, 0));

Console.WriteLine("Last Printed: " + project.Get(Prj.LastPrinted));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


