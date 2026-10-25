---
title: "Filter.CompareTo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Filter. Confronta questa istanza con l'istanza specificata della classe Filter e restituisce un'indicazione del loro ordine relativo"
type: docs
weight: 90
url: /it/net/aspose.tasks/filter/compareto/
---
## Filter.CompareTo method

Confronta questa istanza con l'istanza specificata della classe [`Filter`](../) e restituisce un'indicazione del loro ordine relativo.

```csharp
public int CompareTo(Filter other)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | Filter | l'istanza specificata della classe [`Filter`](../) da confrontare con questo oggetto. |

### Valore di ritorno

un'indicazione del loro ordine relativo.

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


