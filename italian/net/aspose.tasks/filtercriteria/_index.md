---
title: "Classe FilterCriteria"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.FilterCriteria. Definisce i criteri che attività o risorse devono soddisfare per essere visualizzate nella vista MSP"
type: docs
weight: 630
url: /it/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

Definisce i criteri che attività o risorse devono soddisfare per essere visualizzati nella vista MSP.

```csharp
public class FilterCriteria
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | Ottiene l'elenco delle righe figlio `FilterCriteria`. Se il filtro contiene più di una riga di criterio, l'effetto dell'operatore And è che i criteri per entrambe le righe devono essere soddisfatti affinché l'attività o la risorsa venga visualizzata come risultato di questo filtro. L'effetto dell'operatore Or è che i criteri per una delle due righe devono essere soddisfatti. |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | Ottiene o imposta un [`Field`](./field/) da modificare. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | Ottiene o imposta il criterio stabilito con FieldName, Test e Value che si riferisce ad altri criteri nel filtro. |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | Ottiene o imposta il tipo di confronto effettuato tra FieldName e Value che funge da criterio di selezione per il filtro. [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | Ottiene i valori oggetto da confrontare con il valore del campo specificato con FieldName. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [IsFieldValue](../../aspose.tasks/filtercriteria/isfieldvalue/)() | Ottiene se il valore a destra di FilterCriteria è un riferimento a un campo, non un valore costante. |
| [SetValueField](../../aspose.tasks/filtercriteria/setvaluefield/)(Field) | Imposta il campo il cui valore sarà confrontato con il valore del campo specificato da FieldName. |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | Restituisce la rappresentazione stringa dell'istanza della classe `FilterCriteria`. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


