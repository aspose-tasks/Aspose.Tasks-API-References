---
title: "Prj.AdminProject"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, является ли проект административным"
type: docs
weight: 20
url: /ru/net/aspose.tasks/prj/adminproject/
---
## Prj.AdminProject field

Определяет, является ли проект административным проектом.

```csharp
public static readonly Key<NullableBool, PrjKey> AdminProject;
```

## Примеры

Показывает, как читать/записывать свойство Prj.AdminProject.

```csharp
var project = new Project();

project.Set(Prj.AdminProject, true);

Console.WriteLine("Admin Project: " + project.Get(Prj.AdminProject));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


