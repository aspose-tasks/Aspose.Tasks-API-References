---
title: "Asn.BudgetCost"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. Le coût budgété des ressources sur une affectation"
type: docs
weight: 150
url: /fr/net/aspose.tasks/asn/budgetcost/
---
## Asn.BudgetCost field

Le coût budgété des ressources sur une affectation.

```csharp
public static readonly Key<decimal, AsnKey> BudgetCost;
```

## Exemples

Montre comment lire les valeurs de travail/coût budgétées d'une affectation de ressource.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

// Afficher le travail budgété et le coût budgété pour la tâche récapitulative du projet
Console.WriteLine("projSummary.BudgetWork = " + project.RootTask.Get(Tsk.BudgetWork));
Console.WriteLine("projSummary.BudgetCost = " + project.RootTask.Get(Tsk.BudgetCost));

// Afficher le travail budgété de la ressource
var rsc = project.Resources.GetByUid(6);
Console.WriteLine("Resource BudgetWork = " + rsc.Get(Rsc.BudgetWork));

// Afficher le coût budgété de la ressource
rsc = project.Resources.GetByUid(7);
Console.WriteLine("Resource BudgetCost = " + rsc.Get(Rsc.BudgetCost));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var tsk in collector.Tasks)
{
    // Afficher le travail budgété et le coût budgété de l'affectation
    foreach (var assignment in tsk.Assignments)
    {
        var resource = assignment.Get(Asn.Resource);
        if (resource == null)
        {
            continue;
        }

        if (resource.Get(Rsc.Type) == ResourceType.Work)
        {
            Console.WriteLine("Assignment BudgetWork = " + assignment.Get(Asn.BudgetWork));
        }
        else
        {
            Console.WriteLine("Assignment BudgetCost = " + assignment.Get(Asn.BudgetCost));
        }
    }
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


