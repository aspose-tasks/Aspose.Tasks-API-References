---
title: "AssignmentBaseline.CompareTo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "AssignmentBaseline method. Implementazione dell'interfaccia IComparable. Confronta questa istanza con l'oggetto Baseline specificato"
type: docs
weight: 50
url: /it/net/aspose.tasks/assignmentbaseline/compareto/
---
## AssignmentBaseline.CompareTo method

Implementazione dell'interfaccia IComparable. Confronta questa istanza con l'oggetto Baseline specificato.

```csharp
public int CompareTo(AssignmentBaseline other)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| altro | AssignmentBaseline | l'oggetto Baseline specificato con cui confrontare questa istanza. |

### Valore di ritorno

restituisce -1 se questa istanza è inferiore all'oggetto specificato, 1 se questa istanza è superiore all'oggetto specificato; altrimenti restituisce 0

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

* class [AssignmentBaseline](../)
* namespace [Aspose.Tasks](../../assignmentbaseline/)
* assembly [Aspose.Tasks](../../../)


