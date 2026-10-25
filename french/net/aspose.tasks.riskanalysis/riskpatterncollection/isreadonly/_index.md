---
title: "RiskPatternCollection.IsReadOnly"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "RiskPatternCollection propriété. Obtient une valeur indiquant si cette collection est en lecture seule, sinon false"
type: docs
weight: 20
url: /fr/net/aspose.tasks.riskanalysis/riskpatterncollection/isreadonly/
---
## RiskPatternCollection.IsReadOnly property

Obtient une valeur indiquant si cette collection est en lecture seule ; sinon, false.

```csharp
public bool IsReadOnly { get; }
```

## Exemples

Montre comment travailler avec les collections de modèles de risque.

```csharp
var settings = new RiskAnalysisSettings
{
    // Définissez le nombre d'itérations pour la simulation Monte Carlo (la valeur par défaut est 100).
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task1 = project.RootTask.Children.GetById(17);
var task2 = project.RootTask.Children.GetById(18);

// dans la mesure où RiskPatternCollection n'est pas en lecture seule
Console.WriteLine("Is pattern collection read-only?: " + settings.Patterns.IsReadOnly);

// on peut ajouter de nouveaux modèles
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

// itérer sur les modèles ajoutés
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

// modifier le modèle dans la collection en utilisant l'accès par indice
settings.Patterns[task1].Optimistic = 70;
settings.Patterns[task1].Pessimistic = 140;

// vérifier les modèles après les modifications
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

// nous pouvons supprimer le modèle
Console.WriteLine("Removing the first pattern...");
settings.Patterns.Remove(pattern1);

// vérifier que le modèle n'est pas dans la collection
Console.WriteLine("Is collection contains the first pattern?: " + settings.Patterns.Contains(pattern1));

// on peut vider la collection de deux manières

// copier les modèles dans le tableau et les supprimer un par un
var patterns = new RiskPattern[settings.Patterns.Count];
settings.Patterns.CopyTo(patterns, 0);
foreach (var pattern in patterns)
{
    settings.Patterns.Remove(pattern);
}

// ou on peut vider complètement une collection de modèles
settings.Patterns.Clear();
```

### Voir aussi

* class [RiskPatternCollection](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskpatterncollection/)
* assembly [Aspose.Tasks](../../../)


