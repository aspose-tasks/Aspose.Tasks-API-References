---
title: "FilterCriteria.CriteriaRows"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà FilterCriteria. Ottiene l'elenco delle righe figlio di FilterCriteria. Se il filtro contiene più di una riga di criterio, l'effetto di un operatore And è che i criteri per entrambe le righe devono essere soddisfatti affinché l'attività o la risorsa venga visualizzata come risultato di questo filtro. L'effetto di un operatore Or è che i criteri per una delle due righe devono essere soddisfatti"
type: docs
weight: 20
url: /it/net/aspose.tasks/filtercriteria/criteriarows/
---
## FilterCriteria.CriteriaRows property

Ottiene l'elenco delle righe figlio di [`FilterCriteria`](../). Se il filtro contiene più di una riga di criterio, l'effetto di un operatore And è che i criteri per entrambe le righe devono essere soddisfatti affinché l'attività o la risorsa venga visualizzata come risultato di questo filtro. L'effetto di un operatore Or è che i criteri per una delle due righe devono essere soddisfatti.

```csharp
public List<FilterCriteria> CriteriaRows { get; }
```

## Esempi

Mostra come leggere i criteri del filtro attività.

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine("Count of criteria rows: " + filter.Criteria.CriteriaRows.Count);
foreach (var row in filter.Criteria.CriteriaRows)
{
    Console.WriteLine("Field: " + row.Field);
    Console.WriteLine("Operation: " + row.Operation);
    Console.WriteLine("Test: " + row.Test);

    var values = row.Values.Where(c => c != null).ToArray();
    if (values.Length == 0)
    {
        continue;
    }

    Console.WriteLine("Value{0}: {1}", values.Length == 1 ? "" : "s", string.Join(", ", values));
}

// Stampa i criteri del filtro come stringa 
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine("Criteria filter 1:");
Console.WriteLine(criteria1.ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);
Console.WriteLine("Criteria filter 2:");
Console.WriteLine(criteria2.ToString());

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine("Criteria filter 21:");
Console.WriteLine(criteria21.ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine("Criteria filter 22:");
Console.WriteLine(criteria22.ToString());
```

### Vedi anche

* class [FilterCriteria](../)
* namespace [Aspose.Tasks](../../filtercriteria/)
* assembly [Aspose.Tasks](../../../)


