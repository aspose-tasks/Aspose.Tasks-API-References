---
title: "FieldHelper.GetDefaultTaskFieldTitle"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode FieldHelper. Retourne un titre par défaut du champ de tâche spécifique"
type: docs
weight: 20
url: /fr/net/aspose.tasks.util/fieldhelper/getdefaulttaskfieldtitle/
---
## FieldHelper.GetDefaultTaskFieldTitle method

Renvoie un titre par défaut du champ de tâche spécifique.

```csharp
public static string GetDefaultTaskFieldTitle(TaskKey taskKey)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| taskKey | TaskKey | Champ de tâche pour obtenir un titre par défaut. |

### Valeur de retour

Un titre par défaut du champ de tâche spécifique si le champ peut être affiché dans la vue de MS Project, sinon null.

## Exemples

Montre comment obtenir le titre par défaut du champ pour le champ de tâche spécifique.

```csharp
Console.WriteLine("Title for Tsk.ActualCost: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.ActualCost.KeyType));
Console.WriteLine("Title for Tsk.PercentWorkComplete: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.PercentWorkComplete.KeyType));
```

### Voir aussi

* enum [TaskKey](../../../aspose.tasks/taskkey/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


