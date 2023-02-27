---
title: Project.RescheduleUncompletedWorkToStartAfter
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Project méthode. Replanifie les travaux de projet inachevés pour quils commencent après une date spécifiée.
type: docs
weight: 1170
url: /fr/net/aspose.tasks/project/rescheduleuncompletedworktostartafter/
---
## RescheduleUncompletedWorkToStartAfter(DateTime) {#rescheduleuncompletedworktostartafter}

Replanifie les travaux de projet inachevés pour qu'ils commencent après une date spécifiée.

```csharp
public void RescheduleUncompletedWorkToStartAfter(DateTime after)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| after | DateTime | La date à laquelle reprogrammer les travaux inachevés après. |

### Remarques

Assurez-vous que l'indicateur Project.CanSplitsInProgressTasks est défini sur true avant d'utiliser cette méthode.

### Voir également

* class [Project](../)
* espace de noms [Aspose.Tasks](../../project/)
* Assemblée [Aspose.Tasks](../../../)

---

## RescheduleUncompletedWorkToStartAfter(DateTime, List&lt;Task&gt;) {#rescheduleuncompletedworktostartafter_1}

Replanifie le travail inachevé pour une liste spécifiée de tâches à démarrer après une date spécifiée.

```csharp
public void RescheduleUncompletedWorkToStartAfter(DateTime after, List<Task> taskCollection)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| after | DateTime | La date à laquelle reprogrammer les travaux inachevés après. |
| taskCollection | List`1 | List&lt;Task&gt; des tâches pour lesquelles replanifier le travail inachevé. |

### Remarques

Assurez-vous que l'indicateur Project.CanSplitsInProgressTasks est défini sur true avant d'utiliser cette méthode.

### Voir également

* class [Task](../../task/)
* class [Project](../)
* espace de noms [Aspose.Tasks](../../project/)
* Assemblée [Aspose.Tasks](../../../)


