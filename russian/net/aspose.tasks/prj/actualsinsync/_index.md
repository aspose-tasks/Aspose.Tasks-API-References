---
title: "Prj.ActualsInSync"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, были ли все фактические работы синхронизированы с проектом"
type: docs
weight: 10
url: /ru/net/aspose.tasks/prj/actualsinsync/
---
## Prj.ActualsInSync field

Определяет, синхронизированы ли все фактические работы с проектом.

```csharp
public static readonly Key<NullableBool, PrjKey> ActualsInSync;
```

## Примеры

Показывает, как читать/записывать свойство Prj.ActualsInSync.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


