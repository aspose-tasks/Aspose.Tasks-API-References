---
title: "Prj.Autolink"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, автоматически ли связываются вставленные или перемещённые задачи"
type: docs
weight: 70
url: /ru/net/aspose.tasks/prj/autolink/
---
## Prj.Autolink field

Определяет, автоматически связываются ли вставленные или перемещённые задачи.

```csharp
public static readonly Key<NullableBool, PrjKey> Autolink;
```

## Примеры

Показывает, как читать/записывать свойство Prj.Autolink.

```csharp
var project = new Project();

project.Set(Prj.Autolink, true);

Console.WriteLine("Autolink: " + project.Get(Prj.Autolink));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


