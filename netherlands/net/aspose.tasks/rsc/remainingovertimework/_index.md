---
title: "Rsc.RemainingOvertimeWork"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. De hoeveelheid resterende geplande overuren"
type: docs
weight: 600
url: /nl/net/aspose.tasks/rsc/remainingovertimework/
---
## Rsc.RemainingOvertimeWork field

De hoeveelheid resterende geplande overuren.

```csharp
public static readonly Key<Duration, RscKey> RemainingOvertimeWork;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.RemainingOvertimeWork te lezen/schrijven.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + resource.Get(Rsc.RemainingOvertimeWork));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


