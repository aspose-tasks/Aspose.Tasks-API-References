---
title: "Rsc.RemainingWork"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. De tijd die nog nodig is om een taak of een reeks taken te voltooien"
type: docs
weight: 610
url: /nl/net/aspose.tasks/rsc/remainingwork/
---
## Rsc.RemainingWork field

De tijd die nog nodig is om een taak of een reeks taken te voltooien.

```csharp
public static readonly Key<Duration, RscKey> RemainingWork;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.RemainingWork te lezen/schrijven.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + resource.Get(Rsc.RemainingWork));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


