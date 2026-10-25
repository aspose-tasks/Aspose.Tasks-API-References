---
title: "Rsc.IsEnterprise"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Показывает, является ли ресурс из корпоративного пула ресурсов (true) или из локального пула ресурсов (false)"
type: docs
weight: 400
url: /ru/net/aspose.tasks/rsc/isenterprise/
---
## Rsc.IsEnterprise field

Показывает, принадлежит ли ресурс к корпоративному пулу ресурсов (true) или к локальному пулу ресурсов (false).

```csharp
public static readonly Key<NullableBool, RscKey> IsEnterprise;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.IsEnterprise.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsEnterprise, true);

Console.WriteLine("Is Enterprise: " + resource.Get(Rsc.IsEnterprise));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


