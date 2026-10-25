---
title: "Prj.CustomDateFormat"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Пользовательский формат даты представления проекта. Используется для форматирования дат, когда свойство DateFormat установлено в Custom"
type: docs
weight: 200
url: /ru/net/aspose.tasks/prj/customdateformat/
---
## Prj.CustomDateFormat field

Пользовательский формат даты представления проекта. Используется для форматирования дат, когда свойство [`DateFormat`](../dateformat/) установлено в Custom.

```csharp
public static readonly Key<string, PrjKey> CustomDateFormat;
```

## Примеры

Показывает, как читать/записывать свойство Prj.CustomDateFormat.

```csharp
var project = new Project();

project.Set(Prj.CustomDateFormat, "dd MMMM yyyy H:mm");

Console.WriteLine("Custom Date Format: " + project.Get(Prj.CustomDateFormat));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


