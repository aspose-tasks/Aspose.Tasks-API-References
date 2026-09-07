---
title: "Resource.Get"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo di Resource. Restituisce il valore a cui la proprietà è mappata in questo contenitore"
type: docs
weight: 830
url: /it/net/aspose.tasks/resource/get/
---
## Resource.Get&lt;T&gt; method

Restituisce il valore a cui la proprietà è mappata in questo contenitore.

```csharp
public T Get<T>(Key<T, RscKey> key)
```

| Parametro | Descrizione |
| --- | --- |
| T | il tipo del valore mappato. |
| key | la chiave della proprietà specificata. [`Rsc`](../../rsc/) per ottenere la chiave della proprietà. |

### Valore di ritorno

il valore a cui la proprietà è mappata in questo contenitore.

## Esempi

Mostra come leggere/scrivere le proprietà comuni della risorsa.

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
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


