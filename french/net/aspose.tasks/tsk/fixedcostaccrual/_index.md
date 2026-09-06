---
title: "Tsk.FixedCostAccrual"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine les choix concernant comment et quand les coûts fixes doivent être facturés ou imputés au coût d’une tâche"
type: docs
weight: 440
url: /fr/net/aspose.tasks/tsk/fixedcostaccrual/
---
## Tsk.FixedCostAccrual field

Détermine les options pour la façon et le moment où les coûts fixes sont facturés ou accumulés au coût d'une tâche.

```csharp
public static readonly Key<CostAccrualType, TaskKey> FixedCostAccrual;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.FixedCostAccrual.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FixedCostAccrual, CostAccrualType.Prorated);

Console.WriteLine("Fixed Cost Accrual: " + task.Get(Tsk.FixedCostAccrual));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


