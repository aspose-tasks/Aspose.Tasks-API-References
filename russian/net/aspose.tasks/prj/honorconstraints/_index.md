---
title: "Prj.HonorConstraints"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, учитывают ли задачи свои даты ограничений"
type: docs
weight: 370
url: /ru/net/aspose.tasks/prj/honorconstraints/
---
## Prj.HonorConstraints field

Определяет, учитывают ли задачи свои ограничительные даты.

```csharp
public static readonly Key<NullableBool, PrjKey> HonorConstraints;
```

## Примеры

Показывает, как читать/записывать свойство Prj.HonorConstraints.

```csharp
var project = new Project();

project.Set(Prj.HonorConstraints, true);

Console.WriteLine("Honor Constraints: " + project.Get(Prj.HonorConstraints));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


