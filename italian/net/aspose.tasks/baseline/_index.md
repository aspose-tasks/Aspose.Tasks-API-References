---
title: "Classe Baseline"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Baseline. Rappresenta i valori di baseline di una risorsa"
type: docs
weight: 110
url: /it/net/aspose.tasks/baseline/
---
## Baseline class

Rappresenta i valori di baseline di una risorsa.

```csharp
public class Baseline : IComparable<Baseline>, IEquatable<Baseline>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Baseline](baseline/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Ottiene o imposta il numero univoco di un record di dati di baseline. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Ottiene o imposta il costo preventivato di un lavoro eseguito da una risorsa per un progetto fino ad oggi. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Ottiene o imposta il costo preventivo di un lavoro programmato per una risorsa. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Ottiene o imposta il costo previsto di una risorsa quando la baseline viene salvata. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Ottiene o imposta il lavoro assegnato a una risorsa quando la baseline è salvata. La quantità di lavoro assegnato a una risorsa quando la baseline è stata salvata. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | Implementazione dell'interfaccia IComparable. Confronta questa istanza con l'oggetto Baseline specificato. |
| [Equals](../../aspose.tasks/baseline/equals/#equals)(Baseline) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| override [Equals](../../aspose.tasks/baseline/equals/#equals_1)(object) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| override [GetHashCode](../../aspose.tasks/baseline/gethashcode/)() | Restituisce un valore di codice hash per la baseline. |
| [operator ==](../../aspose.tasks/baseline/op_equality/) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [operator &gt;](../../aspose.tasks/baseline/op_greaterthan/) | Restituisce un valore che indica se questa istanza è maggiore di un oggetto specificato. |
| [operator &gt;=](../../aspose.tasks/baseline/op_greaterthanorequal/) | Restituisce un valore che indica se questa istanza è maggiore o uguale a un oggetto specificato. |
| [operator !=](../../aspose.tasks/baseline/op_inequality/) | Restituisce un valore che indica se questa istanza non è uguale a un oggetto specificato. |
| [operator &lt;](../../aspose.tasks/baseline/op_lessthan/) | Restituisce un valore che indica se questa istanza è minore di un oggetto specificato. |
| [operator &lt;=](../../aspose.tasks/baseline/op_lessthanorequal/) | Restituisce un valore che indica se questa istanza è minore o uguale a un oggetto specificato. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


