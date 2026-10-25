---
title: "Asn.BudgetWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Bir göreve ait iş veya malzeme kaynakları için bütçelenen iş miktarı"
type: docs
weight: 160
url: /tr/net/aspose.tasks/asn/budgetwork/
---
## Asn.BudgetWork field

Bir atamadaki iş veya malzeme kaynakları için bütçelenen iş miktarı.

```csharp
public static readonly Key<Duration, AsnKey> BudgetWork;
```

## Örnekler

Bir kaynak atamasının bütçe iş/maliyet değerlerini nasıl okuyacağınızı gösterir.

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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


