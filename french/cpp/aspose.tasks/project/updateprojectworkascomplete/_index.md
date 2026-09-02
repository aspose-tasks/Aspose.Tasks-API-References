---
title: "méthode Aspose::Tasks::Project::UpdateProjectWorkAsComplete"
linktitle: "UpdateProjectWorkAsComplete"
articleTitle: "UpdateProjectWorkAsComplete"
second_title: "Aspose.Tasks pour C++"
description: "Met à jour tout le travail comme terminé jusqu'à une date spécifiée pour l'ensemble du projet."
type: docs
weight: 2080
url: /fr/cpp/aspose.tasks/project/updateprojectworkascomplete/
---

## UpdateProjectWorkAsComplete (1 of 2) {#updateprojectworkascomplete_1}

Met à jour tout le travail comme terminé jusqu'à une date spécifiée pour l'ensemble du projet.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly)
```

| Paramètre | Description |
| --- | --- |
| completeThrough | La date jusqu'à laquelle mettre à jour le travail comme terminé. |
| setZeroOrHundredPercentCompleteOnly | Si défini sur true, ne met à jour que les tâches à 100 % terminées dont la date de fin est antérieure à la date spécifiée. Sinon, calcule une valeur de pourcentage d'achèvement basée sur les dates de début prévues et les dates de fin spécifiées. |

---

## UpdateProjectWorkAsComplete (2 of 2) {#updateprojectworkascomplete_2}

Met à jour tout le travail comme terminé jusqu'à une date spécifiée pour la liste de tâches spécifiée.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Task >>> & taskCollection)
```

| Paramètre | Description |
| --- | --- |
| completeThrough | La date jusqu'à laquelle mettre à jour le travail comme terminé. |
| setZeroOrHundredPercentCompleteOnly | Si défini sur true, ne met à jour que les tâches à 100 % terminées dont la date de fin est antérieure à la date spécifiée. Sinon, calcule une valeur de pourcentage d'achèvement basée sur les dates de début prévues et les dates de fin spécifiées. |
| taskCollection | Liste< Task > des tâches pour lesquelles mettre à jour le travail. |

