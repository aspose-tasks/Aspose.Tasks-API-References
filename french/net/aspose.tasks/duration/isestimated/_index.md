---
title: "Duration.IsEstimated"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Duration. Obtient une valeur indiquant si l'unité de temps est estimée. Le drapeau qui détermine si cette instance Duration est estimée."
type: docs
weight: 30
url: /fr/net/aspose.tasks/duration/isestimated/
---
## Duration.IsEstimated property

Obtient une valeur indiquant si l’unité de temps est estimée. Le drapeau qui détermine si cette instance Duration est estimée.

```csharp
public bool IsEstimated { get; }
```

## Exemples

Montre comment analyser une chaîne à partir d'une chaîne spécialement formatée.

```csharp
var project = new Project();

// exemples de durées :
// "1d", "1dy", "1d?", "1day", "1 dy", "1 edy? ", "8hr", "8 hour", "8hours", "0.2w?", "0.2wk", "0.2 eweek", "0.2ew?"
// où 1 - nombre d'éléments (jour, semaine, etc.), d - jour (h - heure, w - semaine) ? - indicateur estimé, e - indicateur écoulé

// essayer d'analyser une durée estimée
var duration1 = Duration.Parse(project, "1d?");
Console.WriteLine("The parsed time span: " + duration1.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration1.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration1.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration1.IsElapsed);
Console.WriteLine();

// essayer d'analyser une durée estimée
var duration2 = Duration.Parse(project, "0.2 eweek");
Console.WriteLine("The parsed time span: " + duration2.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration2.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration2.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration2.IsElapsed);
```

### Voir aussi

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


