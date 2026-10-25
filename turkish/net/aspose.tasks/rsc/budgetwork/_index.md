---
title: "Rsc.BudgetWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. bütçe çalışması bütçe çalışması ve malzeme kaynakları için. Bütçe kaynakları yalnızca proje özet görevi için atanır."
type: docs
weight: 180
url: /tr/net/aspose.tasks/rsc/budgetwork/
---
## Rsc.BudgetWork field

bütçe işi, bütçe işi ve malzeme kaynakları için. Bütçe kaynakları yalnızca proje özet görevine atanır.

```csharp
public static readonly Key<Duration, RscKey> BudgetWork;
```

## Örnekler

Bir kaynağın bütçe çalışma/maliyet değerlerini nasıl okuyacağını gösterir.

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
foreach (var task in collector.Tasks)
{
    // Atama bütçe çalışmasını ve bütçe maliyetini görüntüle.
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

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


