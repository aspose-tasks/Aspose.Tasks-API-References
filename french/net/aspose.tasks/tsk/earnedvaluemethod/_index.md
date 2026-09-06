---
title: "Tsk.EarnedValueMethod"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Tsk field. Détermine si le champ  Complete ou Physical  Complete doit être utilisé pour calculer le coût budgété du travail effectué BCWP"
type: docs
weight: 350
url: /fr/net/aspose.tasks/tsk/earnedvaluemethod/
---
## Tsk.EarnedValueMethod field

Détermine si le champ % Achevé ou % Physique Achevé doit être utilisé pour calculer le coût budgété du travail effectué (BCWP).

```csharp
public static readonly Key<EarnedValueMethodType, TaskKey> EarnedValueMethod;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.EarnedValueMethod.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarnedValueMethod, EarnedValueMethodType.PercentComplete);

Console.WriteLine("Earned Value Method: " + task.Get(Tsk.EarnedValueMethod));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


