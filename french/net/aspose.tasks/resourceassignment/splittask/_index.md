---
title: ResourceAssignment.SplitTask
second_title: Référence de l'API Aspose.Tasks pour .NET
description: ResourceAssignment méthode. Divise la tâche en deux parties.
type: docs
weight: 750
url: /fr/net/aspose.tasks/resourceassignment/splittask/
---
## ResourceAssignment.SplitTask method

Divise la tâche en deux parties.

```csharp
public void SplitTask(DateTime start, DateTime finish, Calendar calendar)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| start | DateTime | Le début de l'interruption de travail à fractionner en fonction. |
| finish | DateTime | La fin d'interruption de travail à fractionner en fonction. |
| calendar | Calendar | Calendrier sur lequel fractionner. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | Lève lorsque la date de début est antérieure à la date de début de l'affectation. |
| ArgumentOutOfRangeException | Lève lorsque la date de fin est supérieure à la date de fin de l'affectation. |

### Voir également

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* espace de noms [Aspose.Tasks](../../resourceassignment/)
* Assemblée [Aspose.Tasks](../../../)


