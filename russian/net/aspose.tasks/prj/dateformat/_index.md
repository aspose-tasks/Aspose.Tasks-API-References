---
title: "Prj.DateFormat"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Формат даты представления проекта"
type: docs
weight: 210
url: /ru/net/aspose.tasks/prj/dateformat/
---
## Prj.DateFormat field

Формат даты в представлении проекта.

```csharp
public static readonly Key<DateFormat, PrjKey> DateFormat;
```

## Примеры

Показывает, как читать/записывать свойство Prj.DateFormat.

```csharp
var project = new Project();

project.Set(Prj.DateFormat, DateFormat.DateDd);

Console.WriteLine("Date Format: " + project.Get(Prj.DateFormat));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [DateFormat](../../dateformat/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


