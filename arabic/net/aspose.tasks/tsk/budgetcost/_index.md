---
title: "Tsk.BudgetCost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. تكاليف الميزانية للموارد ذات تكلفة الميزانية. يتم تعيين موارد الميزانية فقط لمهمة ملخص المشروع."
type: docs
weight: 140
url: /ar/net/aspose.tasks/tsk/budgetcost/
---
## Tsk.BudgetCost field

تكاليف الميزانية للموارد ذات تكلفة الميزانية. يتم تعيين موارد الميزانية فقط لمهمة ملخص المشروع.

```csharp
public static readonly Key<decimal, TaskKey> BudgetCost;
```

## الأمثلة

يوضح كيفية قراءة قيم العمل/التكلفة الميزانية للمهمة/المورد/التعيين.

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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


