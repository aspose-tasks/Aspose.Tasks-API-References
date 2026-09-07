---
title: "Rsc.MaxUnits"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Il numero massimo di unità che rappresentano la capacità massima per la quale una risorsa è disponibile per svolgere qualsiasi attività durante il periodo di tempo corrente"
type: docs
weight: 450
url: /it/net/aspose.tasks/rsc/maxunits/
---
## Rsc.MaxUnits field

Il numero massimo di unità che rappresentano la capacità massima per cui una risorsa è disponibile per svolgere qualsiasi attività durante il periodo di tempo corrente.

```csharp
public static readonly Key<double, RscKey> MaxUnits;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.MaxUnits.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaxUnits, 2);

Console.WriteLine("Max Units: " + resource.Get(Rsc.MaxUnits));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


