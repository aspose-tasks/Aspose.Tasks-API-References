---
title: "Classe RiskAnalysisResult"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.RiskAnalysis.RiskAnalysisResult. Représente un résultat d'analyse de risque"
type: docs
weight: 1870
url: /fr/net/aspose.tasks.riskanalysis/riskanalysisresult/
---
## RiskAnalysisResult class

Représente un résultat d'analyse des risques.

```csharp
public class RiskAnalysisResult
```

## Méthodes

| Nom | Description |
| --- | --- |
| [GetRiskItems](../../aspose.tasks.riskanalysis/riskanalysisresult/getriskitems/)(RiskItemType) | Renvoie une instance de la collection [`RiskItemStatisticsCollection`](../riskitemstatisticscollection/) pour le type de risque spécifié. |
| [SaveReport](../../aspose.tasks.riskanalysis/riskanalysisresult/savereport/#savereport)(Stream) | Enregistre le rapport d'analyse de risque dans le flux au format PDF. |
| [SaveReport](../../aspose.tasks.riskanalysis/riskanalysisresult/savereport/#savereport_1)(string) | Enregistre le rapport d'analyse de risque à l'emplacement de fichier spécifié au format PDF. |

## Exemples

Montre comment calculer les statistiques des risques et les enregistrer sous forme de rapport PDF.

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

// enregistrer l'analyse sous forme de rapport dans un fichier par chemin d'accès
analysisResult.SaveReport(OutDir + "AnalysisResult_out.pdf");

// ou enregistrer l'analyse dans un flux
using (var stream = new FileStream(OutDir + "AnalysisResult_out1.pdf", FileMode.Create))
{
    analysisResult.SaveReport(stream);
}
```

### Voir aussi

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


