---
title: Class RiskPattern
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Aspose.Tasks.RiskAnalysis.RiskPattern classe. Représente un modèle de risque pour une tâche de projet.
type: docs
weight: 1670
url: /fr/net/aspose.tasks.riskanalysis/riskpattern/
---
## RiskPattern class

Représente un modèle de risque pour une tâche de projet.

```csharp
public class RiskPattern
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [RiskPattern](riskpattern/)(Task) | Initialise une nouvelle instance du`RiskPattern` classe. |

## Propriétés

| Nom | La description |
| --- | --- |
| [ConfidenceLevel](../../aspose.tasks.riskanalysis/riskpattern/confidencelevel/) { get; set; } | Obtient ou définit le niveau de confiance qui correspond au pourcentage de temps pendant lequel les valeurs réelles générées seront comprises entre les estimations optimistes et pessimistes. La valeur par défaut est CL99. |
| [Distribution](../../aspose.tasks.riskanalysis/riskpattern/distribution/) { get; set; } | Obtient ou définit la distribution de probabilité utilisée dans la simulation Monte Carlo. La valeur par défaut est ProbabilityDistributionType.Normal. |
| [Optimistic](../../aspose.tasks.riskanalysis/riskpattern/optimistic/) { get; set; } | Obtient ou définit le pourcentage de la durée de tâche la plus probable qui peut se produire dans le meilleur scénario de projet possible. La valeur par défaut est 75, ce qui signifie que si la durée estimée de la tâche spécifiée est de 4 jours, la durée optimiste sera de 3 jours. |
| [Pessimistic](../../aspose.tasks.riskanalysis/riskpattern/pessimistic/) { get; set; } | Obtient ou définit le pourcentage de la durée de tâche la plus probable qui peut se produire dans le pire scénario de projet possible. La valeur par défaut est 125, ce qui signifie que si la durée estimée de la tâche spécifiée est de 4 jours, la durée pessimiste sera de 5 jours. |
| [Task](../../aspose.tasks.riskanalysis/riskpattern/task/) { get; } | Obtient une tâche de projet à laquelle ce modèle de risque est appliqué. |

### Voir également

* espace de noms [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* Assemblée [Aspose.Tasks](../../)


