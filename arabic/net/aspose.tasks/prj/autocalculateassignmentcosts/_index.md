---
title: "Prj.AutoCalculateAssignmentCosts"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كان يجب حساب تكلفة التكليف والتكلفة المتبقية تلقائيًا باستخدام عمل التكليفات ومعدلات الموارد"
type: docs
weight: 60
url: /ar/net/aspose.tasks/prj/autocalculateassignmentcosts/
---
## Prj.AutoCalculateAssignmentCosts field

يحدد ما إذا كان يجب حساب تكلفة التخصيص والتكلفة المتبقية تلقائيًا باستخدام عمل التخصيص ومعدلات الموارد.

```csharp
public static readonly Key<bool, PrjKey> AutoCalculateAssignmentCosts;
```

## الأمثلة

يظهر كيفية إيقاف الحساب التلقائي لتكاليف التعيين وتعيين تكاليف التعيين يدويًا.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("New task");
task.Duration = project.GetDuration(TimeSpan.FromHours(15), TimeUnitType.Day);
var resource = project.Resources.Add("Resource");
resource.StandardRate = 10m;

var assignment = project.ResourceAssignments.Add(task, resource);

assignment.Work = project.GetDuration(TimeSpan.FromHours(12), TimeUnitType.Day);
assignment.ActualWork = project.GetDuration(TimeSpan.FromHours(3), TimeUnitType.Day);

Console.WriteLine("Now assignment's cost are auto calculated:");
Console.WriteLine("Actual Cost: {0}", assignment.ActualCost);
Console.WriteLine("Remaining Cost: {0}", assignment.RemainingCost);
Console.WriteLine("Cost: {0}", assignment.Cost);

project.AutoCalculateAssignmentCosts = false;
assignment.ActualCost = 123;
assignment.RemainingCost = 456;
assignment.Cost = 555;

Console.WriteLine("Now auto calculation of assignment's cost is turned off.");
Console.WriteLine("Actual Cost: {0}", assignment.ActualCost);
Console.WriteLine("Remaining Cost: {0}", assignment.RemainingCost);
Console.WriteLine("Cost: {0}", assignment.Cost);
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


