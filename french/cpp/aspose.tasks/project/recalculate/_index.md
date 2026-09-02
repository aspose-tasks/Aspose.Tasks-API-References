---
title: "Aspose::Tasks::Project::Recalculate méthode"
linktitle: "Recalculer"
articleTitle: "Recalculer"
second_title: "Aspose.Tasks pour C++"
description: "Replanifie tous les identifiants des tâches du projet, les niveaux de plan, les dates de début/fin, définit les dates anticipées/retardées, calcule les marges, le travail et les champs de coût."
type: docs
weight: 1130
url: /fr/cpp/aspose.tasks/project/recalculate/
---

## Recalculate (1 of 2) {#recalculate_1}

Replanifie tous les identifiants des tâches du projet, les niveaux de plan, les dates de début/fin, définit les dates anticipées/retardées, calcule les marges, le travail et les champs de coût.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate()
```

---

## Recalculate (2 of 2) {#recalculate_2}

Replanifie tous les identifiants des tâches du projet, les niveaux de hiérarchie, les dates de début/fin, définit les dates au plus tôt/au plus tard, calcule les marges, le travail et les champs de coût avec une validation facultative.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate(bool validate)
```

| Paramètre | Description |
| --- | --- |
| valider | Si vrai, la validation du recalcul sera effectuée. Quelles données sont validées : pour le moment, seule la validation de base des plages de dates des tâches et des liaisons de tâches est implémentée. Les plages de dates des tâches (par ex. ActualStart - ActualFinish, EarlyStart - EarlyFinish, etc.) ainsi que les dates des liaisons de tâches seront vérifiées selon le critère selon lequel la date de début est inférieure ou égale à la date de fin. Si l’une des conditions décrites ci‑dessus échoue, alors une RecalculationValidationException sera levée. |

