---
title: "RiskAnalyzer.RiskAnalyzer"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur RiskAnalyzer. Initialise une nouvelle instance de la classe RiskAnalyzer"
type: docs
weight: 10
url: /fr/net/aspose.tasks.riskanalysis/riskanalyzer/riskanalyzer/
---
## RiskAnalyzer constructor

Initialise une nouvelle instance de la classe [`RiskAnalyzer`](../).

```csharp
public RiskAnalyzer(RiskAnalysisSettings settings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| settings | RiskAnalysisSettings | l'instance spécifiée de la classe [`RiskAnalysisSettings`](../../riskanalysissettings/). |

## Exemples

Montre comment démarrer l'analyse des risques en utilisant &lt;see cref="Aspose.Tasks.RiskAnalysis.RiskAnalysisSettings" /&gt;.

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
var earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

settings = new RiskAnalysisSettings
{
    IterationsCount = 300
};

// modifier les paramètres
analyzer.Settings = settings;

analysisResult = analyzer.Analyze(project);
earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### Voir aussi

* class [RiskAnalysisSettings](../../riskanalysissettings/)
* class [RiskAnalyzer](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskanalyzer/)
* assembly [Aspose.Tasks](../../../)


