---
title: "Filter.op_GreaterThan"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Filter. Restituisce un valore che indica se questa istanza è maggiore di un oggetto specificato"
type: docs
weight: 130
url: /it/net/aspose.tasks/filter/op_greaterthan/
---
## Filter GreaterThan operator

Restituisce un valore che indica se questa istanza è maggiore di un oggetto specificato.

```csharp
public static bool operator >(Filter a, Filter b)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | Filter | Il primo filtro. |
| b | Filter | Il secondo filtro. |

### Valore di ritorno

un valore che indica se questa istanza è maggiore di un oggetto specificato

## Esempi

Mostra come verificare l'uguaglianza del filtro.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();

var filter1 = filters[0];
var filter2 = filters[1];

// l'uguaglianza dei filtri viene verificata rispetto all'UID del filtro.
Console.WriteLine("Filter 1 UID: " + filter1.Uid);
Console.WriteLine("Filter 2 UID: " + filter2.Uid);
Console.WriteLine("Are filters equal: " + filter1.Equals(filter2));
```

### Vedi anche

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


