---
title: "Rsc.Work"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De totale hoeveelheid tijd die voor een resource op een taak is gepland."
type: docs
weight: 690
url: /nl/net/aspose.tasks/rsc/work/
---
## Rsc.Work field

De totale hoeveelheid tijd die voor een resource op een taak is gepland.

```csharp
public static readonly Key<Duration, RscKey> Work;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.Work te lezen/schrijven.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Work, project.GetWork(1));

Console.WriteLine("Work: " + resource.Get(Rsc.Work));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


