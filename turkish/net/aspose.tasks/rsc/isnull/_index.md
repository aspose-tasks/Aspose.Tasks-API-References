---
title: "Rsc.IsNull"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın null olup olmadığını belirler."
type: docs
weight: 420
url: /tr/net/aspose.tasks/rsc/isnull/
---
## Rsc.IsNull field

Bir kaynağın null olup olmadığını belirler.

```csharp
public static readonly Key<NullableBool, RscKey> IsNull;
```

## Örnekler

Rsc.IsNull özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsNull, true);

Console.WriteLine("Is Null: " + resource.Get(Rsc.IsNull));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


