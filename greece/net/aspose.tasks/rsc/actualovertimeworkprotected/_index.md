---
title: "Rsc.ActualOvertimeWorkProtected"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το ποσό εργασίας μέσω του οποίου προστατεύεται η πραγματική υπερωριακή εργασία"
type: docs
weight: 60
url: /el/net/aspose.tasks/rsc/actualovertimeworkprotected/
---
## Rsc.ActualOvertimeWorkProtected field

Το ποσό εργασίας μέσω του οποίου προστατεύεται η πραγματική υπερωριακή εργασία.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWorkProtected;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.ActualOvertimeWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + resource.Get(Rsc.ActualOvertimeWorkProtected));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


