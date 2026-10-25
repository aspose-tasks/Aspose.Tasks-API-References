---
title: "Rsc.PeakUnits"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc field. Het maximale toewijzingseenheid voor een resource op elk moment voor alle taken waaraan de resource is toegewezen"
type: docs
weight: 540
url: /nl/net/aspose.tasks/rsc/peakunits/
---
## Rsc.PeakUnits field

De maximale toewijzingseenheid voor een resource op elk moment voor alle taken waaraan de resource is toegewezen.

```csharp
public static readonly Key<double, RscKey> PeakUnits;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.PeakUnits te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.PeakUnits, 2);

Console.WriteLine("Peak Units: " + resource.Get(Rsc.PeakUnits));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


