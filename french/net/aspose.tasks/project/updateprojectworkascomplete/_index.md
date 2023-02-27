---
title: Project.UpdateProjectWorkAsComplete
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Project méthode. Met à jour tous les travaux comme terminés jusquà une date spécifiée pour lensemble du projet.
type: docs
weight: 1250
url: /fr/net/aspose.tasks/project/updateprojectworkascomplete/
---
## UpdateProjectWorkAsComplete(DateTime, bool) {#updateprojectworkascomplete}

Met à jour tous les travaux comme terminés jusqu'à une date spécifiée pour l'ensemble du projet.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| completeThrough | DateTime | La date de mise à jour du travail terminé jusqu'au. |
| setZeroOrHundredPercentCompleteOnly | Boolean | S'il est défini sur true, seules les tâches sont terminées à 100 % dont la date de fin est antérieure à la date d'achèvement spécifiée. Sinon, calcule une valeur de pourcentage d'achèvement en fonction des dates de début et d'achèvement planifiées. |

### Voir également

* class [Project](../)
* espace de noms [Aspose.Tasks](../../project/)
* Assemblée [Aspose.Tasks](../../../)

---

## UpdateProjectWorkAsComplete(DateTime, bool, List&lt;Task&gt;) {#updateprojectworkascomplete_1}

Met à jour tous les travaux comme terminés jusqu'à une date spécifiée pour la liste de tâches spécifiée.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly, List<Task> taskCollection)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| completeThrough | DateTime | La date de mise à jour du travail terminé jusqu'au. |
| setZeroOrHundredPercentCompleteOnly | Boolean | S'il est défini sur true, seules les tâches sont terminées à 100 % dont la date de fin est antérieure à la date d'achèvement spécifiée. Sinon, calcule une valeur de pourcentage d'achèvement en fonction des dates de début et d'achèvement planifiées. |
| taskCollection | List`1 | List&lt;Task&gt; des tâches pour lesquelles mettre à jour le travail. |

### Voir également

* class [Task](../../task/)
* class [Project](../)
* espace de noms [Aspose.Tasks](../../project/)
* Assemblée [Aspose.Tasks](../../../)


