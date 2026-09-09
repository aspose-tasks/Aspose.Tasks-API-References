---
title: "Rsc.RemainingOvertimeWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Kalan planlanmış fazla mesainin miktarı"
type: docs
weight: 600
url: /tr/net/aspose.tasks/rsc/remainingovertimework/
---
## Rsc.RemainingOvertimeWork field

Kalan planlı fazla mesai miktarı.

```csharp
public static readonly Key<Duration, RscKey> RemainingOvertimeWork;
```

## Örnekler

Rsc.RemainingOvertimeWork özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + resource.Get(Rsc.RemainingOvertimeWork));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


