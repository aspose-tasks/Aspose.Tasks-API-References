---
title: "Tsk.BudgetCost"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Κόστη προϋπολογισμού για πόρους προϋπολογισμού. Οι πόροι προϋπολογισμού ανατίθενται μόνο στην εργασία σύνοψης του έργου."
type: docs
weight: 140
url: /el/net/aspose.tasks/tsk/budgetcost/
---
## Tsk.BudgetCost field

Κόστη προϋπολογισμού για πόρους προϋπολογισμού κόστους. Οι πόροι προϋπολογισμού ανατίθενται μόνο στην εργασία σύνοψης του έργου.

```csharp
public static readonly Key<decimal, TaskKey> BudgetCost;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις τιμές προϋπολογισμένης εργασίας/κόστους της εργασίας/πόρου/ανάθεσης.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

// Εμφανίζει την εργασία προϋπολογισμού και το κόστος προϋπολογισμού για την εργασία περίληψης του έργου
Console.WriteLine("projSummary.BudgetWork = " + project.RootTask.Get(Tsk.BudgetWork));
Console.WriteLine("projSummary.BudgetCost = " + project.RootTask.Get(Tsk.BudgetCost));

// Εμφανίζει την εργασία προϋπολογισμού του πόρου
var rsc = project.Resources.GetByUid(6);
Console.WriteLine("Resource BudgetWork = " + rsc.Get(Rsc.BudgetWork));

// Εμφανίζει το κόστος προϋπολογισμού του πόρου
rsc = project.Resources.GetByUid(7);
Console.WriteLine("Resource BudgetCost = " + rsc.Get(Rsc.BudgetCost));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var tsk in collector.Tasks)
{
    // Εμφανίζει την εργασία προϋπολογισμού ανάθεσης και το κόστος προϋπολογισμού
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

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


