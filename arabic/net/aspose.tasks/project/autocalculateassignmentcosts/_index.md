---
title: "Project.AutoCalculateAssignmentCosts"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. تحصل أو تعين ما إذا كان يجب حساب تكلفة التعيين والتكلفة المتبقية تلقائيًا باستخدام عمل التعيينات ومعدلات الموارد"
type: docs
weight: 70
url: /ar/net/aspose.tasks/project/autocalculateassignmentcosts/
---
## Project.AutoCalculateAssignmentCosts property

يحصل أو يعيّن ما إذا كان يجب حساب تكلفة التعيين والتكلفة المتبقية تلقائيًا باستخدام عمل التعيين ومعدلات الموارد.

```csharp
public bool AutoCalculateAssignmentCosts { get; set; }
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

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


