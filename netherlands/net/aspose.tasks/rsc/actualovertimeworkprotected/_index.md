---
title: "Rsc.ActualOvertimeWorkProtected"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De hoeveelheid werk waarvoor daadwerkelijke overuren beschermd zijn"
type: docs
weight: 60
url: /nl/net/aspose.tasks/rsc/actualovertimeworkprotected/
---
## Rsc.ActualOvertimeWorkProtected field

De hoeveelheid werk waardoor werkelijke overuren beschermd zijn.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWorkProtected;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.ActualOvertimeWorkProtected te lezen/schrijven.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + resource.Get(Rsc.ActualOvertimeWorkProtected));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


