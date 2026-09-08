---
title: "Prj.AutoCalculateAssignmentCosts"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 할당 작업 및 리소스 요금을 사용하여 할당 비용 및 남은 비용을 자동으로 계산할지 여부를 결정합니다"
type: docs
weight: 60
url: /ko/net/aspose.tasks/prj/autocalculateassignmentcosts/
---
## Prj.AutoCalculateAssignmentCosts field

할당 작업 및 리소스 요율을 사용하여 할당 비용과 남은 비용을 자동으로 계산할지 여부를 결정합니다.

```csharp
public static readonly Key<bool, PrjKey> AutoCalculateAssignmentCosts;
```

## 예제

할당 비용의 자동 계산을 끄고 할당 비용을 명시적으로 설정하는 방법을 보여줍니다.

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

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


