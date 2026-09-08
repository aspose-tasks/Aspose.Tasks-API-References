---
title: "Prj.CreationDate"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Дата и время создания проекта"
type: docs
weight: 130
url: /ru/net/aspose.tasks/prj/creationdate/
---
## Prj.CreationDate field

Дата и время создания проекта.

```csharp
public static readonly Key<DateTime, PrjKey> CreationDate;
```

## Примечания

Сохранено в формате UTC в файлах mpp. Тип DateTime.

## Примеры

Показывает, как читать/записывать свойство Prj.CreationDate.

```csharp
var project = new Project();

project.Set(Prj.CreationDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Creation Date: " + project.Get(Prj.CreationDate));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


