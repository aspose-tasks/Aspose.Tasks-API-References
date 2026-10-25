---
title: "RiskPattern"
second_title: "Aspose.Tasks pour Python via .NET Référence de l'API"
description: 
type: docs
weight: 60
url: /fr/python-net/aspose.tasks.riskanalysis/riskpattern/
---

## RiskPattern class

Représente un modèle de risque pour une tâche de projet.

Le type RiskPattern expose les membres suivants :
## Constructeurs
| Nom | Description |
| :- | :- |
| RiskPattern(task) | Initialise une nouvelle instance de la classe [RiskPattern](/tasks/python-net/aspose.tasks.riskanalysis/riskpattern/). |
## Propriétés
| Nom | Description |
| :- | :- |
| task | Obtient une tâche de projet à laquelle ce modèle de risque est appliqué. |
| distribution | Obtient ou définit la distribution de probabilité utilisée dans la simulation Monte Carlo.<br/>            La valeur par défaut est ProbabilityDistributionType.Normal. |
| confidence_level | Obtient ou définit le niveau de confiance qui correspond au pourcentage du temps où les valeurs générées réelles seront comprises entre les estimations optimistes et pessimistes.<br/>            La valeur par défaut est CL99. |
| optimistic | Obtient ou définit le pourcentage de la durée de tâche la plus probable qui peut se produire dans le meilleur scénario de projet possible.<br/>            La valeur par défaut est 75, ce qui signifie que si la durée de tâche estimée spécifiée est de 4 jours, alors la durée optimiste sera de 3 jours. |
| pessimistic | Obtient ou définit le pourcentage de la durée de tâche la plus probable qui peut se produire dans le pire scénario de projet possible.<br/>            La valeur par défaut est 125, ce qui signifie que si la durée de tâche estimée spécifiée est de 4 jours, alors la durée pessimiste sera de 5 jours. |

### Voir aussi

* namespace [aspose.tasks.riskanalysis](/tasks/python-net/aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](/tasks/python-net/)

