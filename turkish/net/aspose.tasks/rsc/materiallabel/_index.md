---
title: "Rsc.MaterialLabel"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Malzeme kaynağı için ölçü birimi"
type: docs
weight: 440
url: /tr/net/aspose.tasks/rsc/materiallabel/
---
## Rsc.MaterialLabel field

Malzeme kaynağı için ölçü birimi.

```csharp
public static readonly Key<string, RscKey> MaterialLabel;
```

## Örnekler

Rsc.MaterialLabel özelliğini okuma/yazma yöntemini gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaterialLabel, "kg");

Console.WriteLine("Material Label: " + resource.Get(Rsc.MaterialLabel));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


