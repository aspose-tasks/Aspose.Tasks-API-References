---
title: "Prj.Guid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. GUID проекта"
type: docs
weight: 360
url: /ru/net/aspose.tasks/prj/guid/
---
## Prj.Guid field

GUID проекта.

```csharp
public static readonly Key<Guid, PrjKey> Guid;
```

## Примеры

Показывает, как читать/записывать свойство Prj.Guid.

```csharp
var project = new Project();

project.Set(Prj.Guid, new Guid("efcc0d63-d8e0-4a34-9f3e-9f973f50238a"));

Console.WriteLine("Guid: " + project.Get(Prj.Guid));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


