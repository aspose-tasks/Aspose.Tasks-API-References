---
title: "Rsc.ActualOvertimeWorkProtected"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Gerçek fazla mesai çalışmasının korunduğu iş miktarı"
type: docs
weight: 60
url: /tr/net/aspose.tasks/rsc/actualovertimeworkprotected/
---
## Rsc.ActualOvertimeWorkProtected field

Gerçek fazla mesai çalışmasının korunduğu iş miktarı.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWorkProtected;
```

## Örnekler

Rsc.ActualOvertimeWorkProtected özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + resource.Get(Rsc.ActualOvertimeWorkProtected));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


