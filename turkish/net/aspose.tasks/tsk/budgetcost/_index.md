---
title: "Tsk.BudgetCost"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bütçe maliyet kaynakları için bütçe maliyetleri. Bütçe kaynakları yalnızca proje özet görevine atanır."
type: docs
weight: 140
url: /tr/net/aspose.tasks/tsk/budgetcost/
---
## Tsk.BudgetCost field

Bütçe maliyet kaynakları için bütçe maliyetleri. Bütçe kaynakları yalnızca proje özet görevine atanır.

```csharp
public static readonly Key<decimal, TaskKey> BudgetCost;
```

## Örnekler

Görev/kaynak/atanmanın bütçe iş/maliyet değerlerini okuma nasıl gösterir.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

// Proje özet görevi için bütçe çalışmasını ve bütçe maliyetini görüntüle.
Console.WriteLine("projSummary.BudgetWork = " + project.RootTask.Get(Tsk.BudgetWork));
Console.WriteLine("projSummary.BudgetCost = " + project.RootTask.Get(Tsk.BudgetCost));

// Kaynak bütçe çalışmasını görüntüle.
var rsc = project.Resources.GetByUid(6);
Console.WriteLine("Resource BudgetWork = " + rsc.Get(Rsc.BudgetWork));

// Kaynak bütçe maliyetini görüntüle.
rsc = project.Resources.GetByUid(7);
Console.WriteLine("Resource BudgetCost = " + rsc.Get(Rsc.BudgetCost));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var tsk in collector.Tasks)
{
    // Atama bütçe çalışmasını ve bütçe maliyetini görüntüle.
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

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


