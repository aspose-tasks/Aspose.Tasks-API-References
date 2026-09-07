---
title: "Classe RiskPatternCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.RiskAnalysis.RiskPatternCollection class. Rappresenta una collezione contenente le istanze della classe RiskPattern."
type: docs
weight: 1940
url: /it/net/aspose.tasks.riskanalysis/riskpatterncollection/
---
## RiskPatternCollection class

Rappresenta una collezione contenente le istanze della classe [`RiskPattern`](../riskpattern/).

```csharp
public class RiskPatternCollection : ICollection<RiskPattern>, IDictionary<Task, RiskPattern>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks.riskanalysis/riskpatterncollection/count/) { get; } | Ottiene il numero di elementi contenuti in questa collezione. |
| [IsReadOnly](../../aspose.tasks.riskanalysis/riskpatterncollection/isreadonly/) { get; } | Restituisce un valore che indica se questa collezione è di sola lettura; altrimenti, false. |
| [Item](../../aspose.tasks.riskanalysis/riskpatterncollection/item/) { get; } | Ottiene l'istanza della classe [`RiskPattern`](../riskpattern/) per il task specificato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks.riskanalysis/riskpatterncollection/add/)(RiskPattern) | Aggiunge un'istanza della classe [`RiskPattern`](../riskpattern/) a questa collezione. |
| [Clear](../../aspose.tasks.riskanalysis/riskpatterncollection/clear/)() | Rimuove tutti gli elementi da questa collezione. |
| [Contains](../../aspose.tasks.riskanalysis/riskpatterncollection/contains/)(RiskPattern) | Restituisce true se l'elemento specificato è presente in questa collezione; altrimenti, false. |
| [CopyTo](../../aspose.tasks.riskanalysis/riskpatterncollection/copyto/)(RiskPattern[], int) | Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato. |
| [GetEnumerator](../../aspose.tasks.riskanalysis/riskpatterncollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Remove](../../aspose.tasks.riskanalysis/riskpatterncollection/remove/)(RiskPattern) | Rimuove la prima occorrenza di un oggetto specifico da questa collezione. |

## Esempi

Mostra come lavorare con le collezioni di pattern di rischio.

```csharp
var settings = new RiskAnalysisSettings
{
    // Imposta il numero di iterazioni per la simulazione Monte Carlo (il valore predefinito è 100).
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task1 = project.RootTask.Children.GetById(17);
var task2 = project.RootTask.Children.GetById(18);

// per quanto riguarda RiskPatternCollection, non è di sola lettura
Console.WriteLine("Is pattern collection read-only?: " + settings.Patterns.IsReadOnly);

// si possono aggiungere nuovi pattern
var pattern1 = new RiskPattern(task1)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 60,
    Pessimistic = 140,
    ConfidenceLevel = ConfidenceLevel.CL75
};
var pattern2 = new RiskPattern(task2)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 70,
    Pessimistic = 130,
    ConfidenceLevel = ConfidenceLevel.CL75
};

settings.Patterns.Add(pattern1);
settings.Patterns.Add(pattern2);

// iterare sui pattern aggiunti
Console.WriteLine("Patterns count: " + settings.Patterns.Count);
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// modifica il pattern nella collezione usando l'accesso per indice
settings.Patterns[task1].Optimistic = 70;
settings.Patterns[task1].Pessimistic = 140;

// verifica i pattern dopo le modifiche
Console.WriteLine("Print edited patterns: ");
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// possiamo rimuovere il pattern
Console.WriteLine("Removing the first pattern...");
settings.Patterns.Remove(pattern1);

// verifica che il pattern non sia nella collezione
Console.WriteLine("Is collection contains the first pattern?: " + settings.Patterns.Contains(pattern1));

// è possibile svuotare la collezione in due modi

// copia i pattern nell'array e cancellali uno per uno
var patterns = new RiskPattern[settings.Patterns.Count];
settings.Patterns.CopyTo(patterns, 0);
foreach (var pattern in patterns)
{
    settings.Patterns.Remove(pattern);
}

// oppure si può svuotare completamente una collezione di pattern
settings.Patterns.Clear();
```

### Vedi anche

* class [RiskPattern](../riskpattern/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


