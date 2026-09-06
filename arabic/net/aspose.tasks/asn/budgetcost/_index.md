---
title: "Asn.BudgetCost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. التكلفة المتوقعة للموارد في تعيين"
type: docs
weight: 150
url: /ar/net/aspose.tasks/asn/budgetcost/
---
## Asn.BudgetCost field

التكلفة المتوقعة للموارد على المهمة.

```csharp
public static readonly Key<decimal, AsnKey> BudgetCost;
```

## الأمثلة

يظهر كيفية قراءة قيم عمل/تكلفة الميزانية لتعيين مورد.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

// عرض عمل الميزانية وتكلفة الميزانية لمهمة ملخص المشروع
Console.WriteLine("projSummary.BudgetWork = " + project.RootTask.Get(Tsk.BudgetWork));
Console.WriteLine("projSummary.BudgetCost = " + project.RootTask.Get(Tsk.BudgetCost));

// عرض عمل ميزانية المورد
var rsc = project.Resources.GetByUid(6);
Console.WriteLine("Resource BudgetWork = " + rsc.Get(Rsc.BudgetWork));

// عرض تكلفة ميزانية المورد
rsc = project.Resources.GetByUid(7);
Console.WriteLine("Resource BudgetCost = " + rsc.Get(Rsc.BudgetCost));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var tsk in collector.Tasks)
{
    // عرض عمل ميزانية التعيين وتكلفة الميزانية
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

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


