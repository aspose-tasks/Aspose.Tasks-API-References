---
title: "Rsc.PeakUnits"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın atandığı tüm görevler için herhangi bir anda kaynak için maksimum atama birimi"
type: docs
weight: 540
url: /tr/net/aspose.tasks/rsc/peakunits/
---
## Rsc.PeakUnits field

Kaynağın atandığı tüm görevler için herhangi bir zamanda olabilecek maksimum atama birimi.

```csharp
public static readonly Key<double, RscKey> PeakUnits;
```

## Örnekler

Rsc.PeakUnits özelliğini okuma/yazma yöntemini gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.PeakUnits, 2);

Console.WriteLine("Peak Units: " + resource.Get(Rsc.PeakUnits));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


