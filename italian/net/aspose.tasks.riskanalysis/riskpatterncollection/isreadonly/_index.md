---
title: "RiskPatternCollection.IsReadOnly"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà RiskPatternCollection. Ottiene un valore che indica se questa raccolta è di sola lettura; altrimenti false"
type: docs
weight: 20
url: /it/net/aspose.tasks.riskanalysis/riskpatterncollection/isreadonly/
---
## RiskPatternCollection.IsReadOnly property

Restituisce un valore che indica se questa collezione è di sola lettura; altrimenti, false.

```csharp
public bool IsReadOnly { get; }
```

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

* class [RiskPatternCollection](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskpatterncollection/)
* assembly [Aspose.Tasks](../../../)


