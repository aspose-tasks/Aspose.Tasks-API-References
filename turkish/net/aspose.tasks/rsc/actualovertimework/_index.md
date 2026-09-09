---
title: "Rsc.ActualOvertimeWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Görevlere atanan kaynak tarafından zaten yapılan gerçek fazla mesai miktarı."
type: docs
weight: 50
url: /tr/net/aspose.tasks/rsc/actualovertimework/
---
## Rsc.ActualOvertimeWork field

Görevlere atanan kaynak tarafından zaten yapılan fazla mesai çalışmasının gerçek miktarı.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWork;
```

## Örnekler

Rsc.ActualOvertimeWork özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + resource.Get(Rsc.ActualOvertimeWork));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


