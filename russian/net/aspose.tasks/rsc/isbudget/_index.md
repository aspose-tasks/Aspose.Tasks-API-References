---
title: "Rsc.IsBudget"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Определяет, является ли рабочий материал или ресурс затрат бюджетным ресурсом"
type: docs
weight: 380
url: /ru/net/aspose.tasks/rsc/isbudget/
---
## Rsc.IsBudget field

Определяет, является ли рабочий, материал или ресурс затрат бюджетным ресурсом.

```csharp
public static readonly Key<NullableBool, RscKey> IsBudget;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.IsBudget.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsBudget, true);

Console.WriteLine("Is Budget: " + resource.Get(Rsc.IsBudget));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


