---
title: "RiskItemStatistics.ToString"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode RiskItemStatistics. Retourne une représentation sous forme de chaîne courte d’un élément de risque. Les détails exacts de la représentation ne sont pas spécifiés et peuvent changer."
type: docs
weight: 70
url: /fr/net/aspose.tasks.riskanalysis/riskitemstatistics/tostring/
---
## RiskItemStatistics.ToString method

Renvoie une représentation courte sous forme de chaîne d'un élément de risque. Les détails exacts de la représentation ne sont pas spécifiés et peuvent changer.

```csharp
public override string ToString()
```

### Valeur de retour

chaîne courte qui représente l’objet RiskItem.

## Exemples

Montre comment calculer les statistiques des risques.

```csharp
var settings = new RiskAnalysisSettings
{
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Initialiser un modèle de risque
var pattern = new RiskPattern(task)
{
    // Sélectionnez un type de distribution pour le générateur de nombres aléatoires afin de générer des valeurs possibles (seuls deux types sont actuellement pris en charge, à savoir normal et uniforme)
    // Pour plus de détails, voir ici : https://en.wikipedia.org/wiki/Normal_distribution)
    Distribution = ProbabilityDistributionType.Normal,

    // Définissez le pourcentage de la durée de tâche la plus probable qui peut se produire dans le meilleur scénario de projet possible
    // La valeur par défaut est 75, ce qui signifie que si la durée de tâche estimée spécifiée est de 4 jours, alors la durée optimiste sera de 3 jours
    Optimistic = 70,

    // Définissez le pourcentage de la durée de tâche la plus probable qui peut se produire dans le pire scénario de projet possible
    // La valeur par défaut est 125, ce qui signifie que si la durée de tâche estimée spécifiée est de 4 jours, alors la durée pessimiste sera de 5 jours.
    Pessimistic = 130,

    // Définissez un niveau de confiance qui correspond au pourcentage du temps où les valeurs réelles se situeront entre les estimations optimistes et pessimistes.
    // Vous pouvez le considérer comme une valeur d'écart type : plus vous êtes incertain quant à vos estimations, plus la valeur d'écart type utilisée dans le générateur de nombres aléatoires est élevée.
    ConfidenceLevel = ConfidenceLevel.CL75
};
settings.Patterns.Add(pattern);

// Analyser les risques du projet
var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);
var statistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Short statistic: " + statistics);
Console.WriteLine();
Console.WriteLine("Statistic details: ");
Console.WriteLine("Item Type: {0}", statistics.ItemType);
Console.WriteLine("Expected value: {0}", statistics.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", statistics.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", statistics.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", statistics.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", statistics.GetPercentile(90));
Console.WriteLine("Minimum: {0}", statistics.Minimum);
Console.WriteLine("Maximum: {0}", statistics.Maximum);
```

### Voir aussi

* class [RiskItemStatistics](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskitemstatistics/)
* assembly [Aspose.Tasks](../../../)


