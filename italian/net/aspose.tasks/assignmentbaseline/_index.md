---
title: "Classe AssignmentBaseline"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.AssignmentBaseline. Rappresenta la baseline di un'assegnazione di risorsa"
type: docs
weight: 50
url: /it/net/aspose.tasks/assignmentbaseline/
---
## AssignmentBaseline class

Rappresenta la Baseline di un'assegnazione di risorsa.

```csharp
public class AssignmentBaseline : Baseline, IComparable<AssignmentBaseline>, 
    IEquatable<AssignmentBaseline>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [AssignmentBaseline](assignmentbaseline/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Ottiene o imposta il numero univoco di un record di dati di baseline. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Ottiene o imposta il costo preventivato di un lavoro eseguito da una risorsa per un progetto fino ad oggi. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Ottiene o imposta il costo preventivo di un lavoro programmato per una risorsa. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Ottiene o imposta il costo previsto di una risorsa quando la baseline viene salvata. |
| [Finish](../../aspose.tasks/assignmentbaseline/finish/) { get; set; } | Ottiene o imposta la data di fine programmata dell'assegnazione della risorsa quando la baseline è stata salvata. La data di fine dell'assegnazione della risorsa quando questa baseline è stata salvata. |
| [Start](../../aspose.tasks/assignmentbaseline/start/) { get; set; } | Ottiene o imposta la data di inizio programmata dell'assegnazione della risorsa quando la baseline è stata salvata. La data di inizio dell'assegnazione della risorsa quando questa baseline è stata salvata. |
| [TimephasedData](../../aspose.tasks/assignmentbaseline/timephaseddata/) { get; set; } | Ottiene o imposta l'istanza di [`TimephasedDataCollection`](../timephaseddatacollection/) per questo oggetto. I dati temporizzati associati alla baseline dell'assegnazione della risorsa. Restituisce l'istanza di [`TimephasedDataCollection`](../timephaseddatacollection/) per questo oggetto. La raccolta di dati temporizzati associati a questa baseline. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Ottiene o imposta il lavoro assegnato a una risorsa quando la baseline è salvata. La quantità di lavoro assegnato a una risorsa quando la baseline è stata salvata. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CompareTo](../../aspose.tasks/assignmentbaseline/compareto/#compareto)(AssignmentBaseline) | Implementazione dell'interfaccia IComparable. Confronta questa istanza con l'oggetto Baseline specificato. |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | Implementazione dell'interfaccia IComparable. Confronta questa istanza con l'oggetto Baseline specificato. |
| [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals)(AssignmentBaseline) | Restituisce un valore che indica se questa istanza è uguale all'oggetto AssignmentBaseline specificato. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| override [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals_2)(object) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| override [GetHashCode](../../aspose.tasks/assignmentbaseline/gethashcode/)() |  |

## Esempi

Mostra come lavorare con le baseline delle assegnazioni.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// Le baseline delle assegnazioni vengono impostate quando si imposta la baseline sull'intero progetto.
project.SetBaseline(BaselineType.Baseline);

// leggi le informazioni della baseline dell'assegnazione
foreach (var assignment in project.ResourceAssignments)
{
    foreach (var baseline in assignment.Baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
        Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
        if (baseline.TimephasedData != null)
        {
            foreach (var td in baseline.TimephasedData)
            {
                Console.WriteLine("TD Start: " + td.Start);
                Console.WriteLine("TD Finish: " + td.Finish);
                Console.WriteLine("TD Timephased Data Type: " + td.TimephasedDataType);
                Console.WriteLine();
            }
        }

        Console.WriteLine();
    }

    Console.WriteLine();
}

// verifica l'uguaglianza della baseline
var assn1 = project.ResourceAssignments.GetByUid(5);
var assn2 = project.ResourceAssignments.GetByUid(7);

var assignmentBaseline1 = assn1.Baselines.ToList()[0];
var assignmentBaseline2 = assn2.Baselines.ToList()[0];

// le baseline possono essere confrontate usando le sovraccarichi del metodo 'Equals'
Console.WriteLine("Are baselines equal: " + assignmentBaseline1.Equals(assignmentBaseline2));

// oppure usando l'operazione aritmetica sovraccaricata
Console.WriteLine("Is baseline 1 less than baseline 2: " + (assignmentBaseline1 < assignmentBaseline2));

// l'hashcode della baseline è basato sul numero della baseline
Console.WriteLine("Assignment baseline 1 hashcode: " + assignmentBaseline1.GetHashCode());
Console.WriteLine("Assignment baseline 2 hashcode: " + assignmentBaseline2.GetHashCode());
```

### Vedi anche

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


