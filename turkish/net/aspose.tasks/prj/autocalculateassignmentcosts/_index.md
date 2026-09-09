---
title: "Prj.AutoCalculateAssignmentCosts"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Atama maliyetinin ve kalan maliyetin, atama çalışması ve kaynak oranları kullanılarak otomatik olarak hesaplanıp hesaplanmayacağını belirler"
type: docs
weight: 60
url: /tr/net/aspose.tasks/prj/autocalculateassignmentcosts/
---
## Prj.AutoCalculateAssignmentCosts field

Atama maliyeti ve kalan maliyetin, atamanın işi ve kaynak oranları kullanılarak otomatik olarak hesaplanıp hesaplanmayacağını belirler.

```csharp
public static readonly Key<bool, PrjKey> AutoCalculateAssignmentCosts;
```

## Örnekler

Atama maliyetlerinin otomatik hesaplamasını nasıl kapatacağınızı ve maliyetleri açıkça nasıl ayarlayacağınızı gösterir.

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

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


