---
title: "Rsc.IsEnterprise"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın kurumsal kaynak havuzundan (true) mi yoksa yerel kaynak havuzundan (false) mı olduğunu gösterir."
type: docs
weight: 400
url: /tr/net/aspose.tasks/rsc/isenterprise/
---
## Rsc.IsEnterprise field

Bir kaynağın kurumsal kaynak havuzundan (doğru) mı yoksa yerel kaynak havuzundan (yanlış) mı olduğunu gösterir.

```csharp
public static readonly Key<NullableBool, RscKey> IsEnterprise;
```

## Örnekler

Rsc.IsEnterprise özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsEnterprise, true);

Console.WriteLine("Is Enterprise: " + resource.Get(Rsc.IsEnterprise));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


