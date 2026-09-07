---
title: "AssignmentBaseline.TimephasedData"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "AssignmentBaseline property. Ottiene o imposta l'istanza di TimephasedDataCollection per questo oggetto. I dati temporizzati associati alla baseline dell'assegnazione della risorsa. restituisce l'istanza di TimephasedDataCollection per questo oggetto. La collezione di dati temporizzati associata a questa baseline"
type: docs
weight: 40
url: /it/net/aspose.tasks/assignmentbaseline/timephaseddata/
---
## AssignmentBaseline.TimephasedData property

Ottiene o imposta l'istanza di [`TimephasedDataCollection`](../../timephaseddatacollection/) per questo oggetto. I dati temporizzati associati alla baseline dell'assegnazione della risorsa. restituisce l'istanza di [`TimephasedDataCollection`](../../timephaseddatacollection/) per questo oggetto. La collezione di dati temporizzati associata a questa baseline.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

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

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [AssignmentBaseline](../)
* namespace [Aspose.Tasks](../../assignmentbaseline/)
* assembly [Aspose.Tasks](../../../)


