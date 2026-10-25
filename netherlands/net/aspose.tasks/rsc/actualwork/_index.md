---
title: "Rsc.ActualWork"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc field. De hoeveelheid werk die al is uitgevoerd door de aan taken toegewezen resource"
type: docs
weight: 70
url: /nl/net/aspose.tasks/rsc/actualwork/
---
## Rsc.ActualWork field

De hoeveelheid werk die al is gedaan door de aan taken toegewezen resource.

```csharp
public static readonly Key<Duration, RscKey> ActualWork;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.ActualWork te lezen/schrijven.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + resource.Get(Rsc.ActualWork));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


