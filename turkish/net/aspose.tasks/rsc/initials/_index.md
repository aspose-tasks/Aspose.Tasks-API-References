---
title: "Rsc.Initials"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın baş harfleri."
type: docs
weight: 370
url: /tr/net/aspose.tasks/rsc/initials/
---
## Rsc.Initials field

Bir kaynağın baş harfleri.

```csharp
public static readonly Key<string, RscKey> Initials;
```

## Örnekler

Rsc.Initials özelliğini nasıl okuyup yazacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Initials, "R");

Console.WriteLine("Initials: " + resource.Get(Rsc.Initials));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


