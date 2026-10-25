---
title: "Rsc.OvertimeRate"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Il tasso di retribuzione per il lavoro straordinario svolto da una risorsa"
type: docs
weight: 510
url: /it/net/aspose.tasks/rsc/overtimerate/
---
## Rsc.OvertimeRate field

Il tasso di retribuzione per il lavoro straordinario svolto da una risorsa.

```csharp
public static readonly Key<decimal, RscKey> OvertimeRate;
```

## Esempi

Mostra come gestire le tariffe e i gruppi delle risorse.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// Aggiungi risorsa e imposta alcune proprietà
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


