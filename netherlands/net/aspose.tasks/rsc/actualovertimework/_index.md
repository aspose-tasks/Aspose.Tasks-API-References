---
title: "Rsc.ActualOvertimeWork"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De werkelijke hoeveelheid overuren die al door de aan taken toegewezen resource is uitgevoerd."
type: docs
weight: 50
url: /nl/net/aspose.tasks/rsc/actualovertimework/
---
## Rsc.ActualOvertimeWork field

De werkelijke hoeveelheid overuren die al is uitgevoerd door de aan taken toegewezen resource.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWork;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.ActualOvertimeWork te lezen/schrijven.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + resource.Get(Rsc.ActualOvertimeWork));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


