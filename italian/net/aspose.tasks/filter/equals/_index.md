---
title: "Filter.Equals"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Filter. Restituisce un valore che indica se questa istanza è uguale all'oggetto AssignmentBaseline specificato"
type: docs
weight: 100
url: /it/net/aspose.tasks/filter/equals/
---
## Equals(Filter) {#equals}

Restituisce un valore che indica se questa istanza è uguale all'oggetto AssignmentBaseline specificato.

```csharp
public bool Equals(Filter other)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| altro | Filter | l'oggetto AssignmentBaseline specificato da confrontare con questa istanza. |

### Valore di ritorno

restituisce true se questa istanza è uguale all'oggetto AssignmentBaseline specificato; altrimenti, false.

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

---

## Equals(object) {#equals_1}

Restituisce un valore che indica se questa istanza è uguale all'oggetto AssignmentBaseline specificato.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Oggetto | l'oggetto AssignmentBaseline specificato da confrontare con questa istanza. |

### Valore di ritorno

restituisce true se questa istanza è uguale all'oggetto AssignmentBaseline specificato; altrimenti, false.

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


