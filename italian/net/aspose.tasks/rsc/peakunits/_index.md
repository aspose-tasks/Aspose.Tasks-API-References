---
title: "Rsc.PeakUnits"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. L'unità di assegnazione massima per una risorsa in qualsiasi momento per tutti i compiti a cui la risorsa è assegnata"
type: docs
weight: 540
url: /it/net/aspose.tasks/rsc/peakunits/
---
## Rsc.PeakUnits field

L'unità massima di assegnazione per una risorsa in qualsiasi momento per tutte le attività a cui la risorsa è assegnata.

```csharp
public static readonly Key<double, RscKey> PeakUnits;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.PeakUnits.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.PeakUnits, 2);

Console.WriteLine("Peak Units: " + resource.Get(Rsc.PeakUnits));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


