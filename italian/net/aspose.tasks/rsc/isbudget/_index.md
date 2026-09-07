---
title: "Rsc.IsBudget"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Determina se un materiale di lavoro o una risorsa di costo è una risorsa di budget"
type: docs
weight: 380
url: /it/net/aspose.tasks/rsc/isbudget/
---
## Rsc.IsBudget field

Determina se una risorsa di lavoro, materiale o costo è una risorsa di budget.

```csharp
public static readonly Key<NullableBool, RscKey> IsBudget;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.IsBudget.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsBudget, true);

Console.WriteLine("Is Budget: " + resource.Get(Rsc.IsBudget));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


