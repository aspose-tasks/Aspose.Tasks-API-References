---
title: "Rsc.RemainingWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir görevi veya görev setini tamamlamak için hâlâ gereken süre"
type: docs
weight: 610
url: /tr/net/aspose.tasks/rsc/remainingwork/
---
## Rsc.RemainingWork field

Bir görevi veya görev setini tamamlamak için hâlâ gereken süre.

```csharp
public static readonly Key<Duration, RscKey> RemainingWork;
```

## Örnekler

Rsc.RemainingWork özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + resource.Get(Rsc.RemainingWork));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


