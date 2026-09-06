---
title: "Rsc.BudgetWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. عمل الميزانية للعمالة والموارد المادية. تُخصص موارد الميزانية فقط لمهمة ملخص المشروع"
type: docs
weight: 180
url: /ar/net/aspose.tasks/rsc/budgetwork/
---
## Rsc.BudgetWork field

عمل الميزانية للموارد ذات عمل الميزانية والمواد. يتم تعيين موارد الميزانية فقط لمهمة ملخص المشروع.

```csharp
public static readonly Key<Duration, RscKey> BudgetWork;
```

## الأمثلة

يوضح كيفية قراءة قيم عمل/تكلفة الميزانية لمورد.

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
foreach (var task in collector.Tasks)
{
    // عرض عمل ميزانية التعيين وتكلفة الميزانية
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

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


