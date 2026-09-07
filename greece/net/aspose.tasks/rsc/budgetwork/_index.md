---
title: "Rsc.BudgetWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Rsc πεδίο. εργασία προϋπολογισμού για εργασία προϋπολογισμού και υλικούς πόρους. Οι πόροι προϋπολογισμού ανατίθενται μόνο στην εργασία περίληψης του έργου"
type: docs
weight: 180
url: /el/net/aspose.tasks/rsc/budgetwork/
---
## Rsc.BudgetWork field

Προϋπολογισμένη εργασία για προϋπολογισμένη εργασία και υλικούς πόρους. Οι πόροι προϋπολογισμού ανατίθενται μόνο στην εργασία σύνοψης του έργου.

```csharp
public static readonly Key<Duration, RscKey> BudgetWork;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις τιμές εργασίας/κόστους προϋπολογισμού ενός πόρου.

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
foreach (var task in collector.Tasks)
{
    // Εμφανίζει την εργασία προϋπολογισμού ανάθεσης και το κόστος προϋπολογισμού
    foreach (var assignment in task.Assignments)
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
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


