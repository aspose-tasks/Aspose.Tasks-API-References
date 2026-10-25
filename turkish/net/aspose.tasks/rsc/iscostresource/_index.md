---
title: "Rsc.IsCostResource"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın maliyet kaynağı olup olmadığını belirler"
type: docs
weight: 390
url: /tr/net/aspose.tasks/rsc/iscostresource/
---
## Rsc.IsCostResource field

Bir kaynağın maliyet kaynağı olup olmadığını belirler.

```csharp
public static readonly Key<NullableBool, RscKey> IsCostResource;
```

## Örnekler

Rsc.IsCostResource özelliğini okuma/yazma yöntemini gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsCostResource, true);

Console.WriteLine("Is Cost Resource: " + resource.Get(Rsc.IsCostResource));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


