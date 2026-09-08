---
title: "Rsc.RegularWork"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De totale hoeveelheid niet‑overurenwerk die gepland is om door de resource uitgevoerd te worden."
type: docs
weight: 570
url: /nl/net/aspose.tasks/rsc/regularwork/
---
## Rsc.RegularWork field

De totale hoeveelheid niet‑overurenwerk die gepland is om door de resource uitgevoerd te worden.

```csharp
public static readonly Key<Duration, RscKey> RegularWork;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.RegularWork te lezen/schrijven.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + resource.Get(Rsc.RegularWork));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


