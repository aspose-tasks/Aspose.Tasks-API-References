---
title: "Classe Filter"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Filter. Rappresenta un filtro in Project"
type: docs
weight: 600
url: /it/net/aspose.tasks/filter/
---
## Filter class

Rappresenta un filtro in Project.

```csharp
public sealed class Filter : IComparable<Filter>, IEquatable<Filter>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Filter](filter/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Criteria](../../aspose.tasks/filter/criteria/) { get; set; } | Ottiene o imposta i criteri che attività o risorse devono soddisfare per essere visualizzati nella vista MSP. |
| [FilterType](../../aspose.tasks/filter/filtertype/) { get; set; } | Ottiene il tipo del filtro. |
| [Index](../../aspose.tasks/filter/index/) { get; } | Ottiene l'indice di un oggetto `Filter` nell'oggetto contenitore dei Filtri. |
| [Name](../../aspose.tasks/filter/name/) { get; set; } | Ottiene o imposta il nome di un oggetto Filter. |
| [ShowInMenu](../../aspose.tasks/filter/showinmenu/) { get; set; } | Ottiene o imposta un valore che indica se il progetto mostra il nome del filtro nell'elenco a discesa Filter nella scheda Visualizza del Ribbon. |
| [ShowRelatedSummaryRows](../../aspose.tasks/filter/showrelatedsummaryrows/) { get; set; } | Ottiene o imposta un valore che indica se le righe di riepilogo correlate sono visualizzate per il filtro. |
| [Uid](../../aspose.tasks/filter/uid/) { get; } | Ottiene l'identificatore univoco di un filtro. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CompareTo](../../aspose.tasks/filter/compareto/)(Filter) | Confronta questa istanza con l'istanza specificata della classe `Filter` e restituisce un'indicazione del loro ordine relativo. |
| [Equals](../../aspose.tasks/filter/equals/#equals)(Filter) | Restituisce un valore che indica se questa istanza è uguale all'oggetto AssignmentBaseline specificato. |
| override [Equals](../../aspose.tasks/filter/equals/#equals_1)(object) | Restituisce un valore che indica se questa istanza è uguale all'oggetto AssignmentBaseline specificato. |
| override [GetHashCode](../../aspose.tasks/filter/gethashcode/)() | Restituisce un valore di codice hash per il filtro. |
| [operator ==](../../aspose.tasks/filter/op_equality/) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [operator &gt;](../../aspose.tasks/filter/op_greaterthan/) | Restituisce un valore che indica se questa istanza è maggiore di un oggetto specificato. |
| [operator &gt;=](../../aspose.tasks/filter/op_greaterthanorequal/) | Restituisce un valore che indica se questa istanza è maggiore o uguale a un oggetto specificato. |
| [operator !=](../../aspose.tasks/filter/op_inequality/) | Restituisce un valore che indica se questa istanza non è uguale a un oggetto specificato. |
| [operator &lt;](../../aspose.tasks/filter/op_lessthan/) | Restituisce un valore che indica se questa istanza è minore di un oggetto specificato. |
| [operator &lt;=](../../aspose.tasks/filter/op_lessthanorequal/) | Restituisce un valore che indica se questa istanza è minore o uguale a un oggetto specificato. |

## Esempi

Mostra come lavorare con i filtri.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();
Console.WriteLine("Task filters count: " + filters.Count);
foreach (var filter in filters)
{
    Console.WriteLine("Uid: " + filter.Uid);
    Console.WriteLine("Index: " + filter.Index);
    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

// verifica i filtri delle risorse
List<Filter> resourceFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + resourceFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + resourceFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + resourceFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + resourceFilters[0].ShowRelatedSummaryRows);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


