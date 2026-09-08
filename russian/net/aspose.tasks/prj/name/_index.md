---
title: "Prj.Name"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Имя проекта"
type: docs
weight: 540
url: /ru/net/aspose.tasks/prj/name/
---
## Prj.Name field

Имя проекта.

```csharp
public static readonly Key<string, PrjKey> Name;
```

## Примеры

Показывает, как читать/записывать название проекта.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

project.Set(Prj.Name, "Custom Project Name");

Console.WriteLine("Project name: " + project.Get(Prj.Name));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


