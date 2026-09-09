---
title: "Project.AutoCalculateAssignmentCosts"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. Atama maliyeti ve kalan maliyetin, atama çalışması ve kaynak oranları kullanılarak otomatik olarak hesaplanıp hesaplanmayacağını alır veya ayarlar."
type: docs
weight: 70
url: /tr/net/aspose.tasks/project/autocalculateassignmentcosts/
---
## Project.AutoCalculateAssignmentCosts property

Atama maliyeti ve kalan maliyetin, atamanın işi ve kaynak oranları kullanılarak otomatik olarak hesaplanıp hesaplanmayacağını alır veya ayarlar.

```csharp
public bool AutoCalculateAssignmentCosts { get; set; }
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

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


