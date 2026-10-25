---
title: "Rsc.Overallocated"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스가 특정 작업 또는 모든 작업에 대해 정상 작업 용량 내에서 완료할 수 있는 것보다 더 많은 작업이 할당되었는지 여부를 나타냅니다."
type: docs
weight: 490
url: /ko/net/aspose.tasks/rsc/overallocated/
---
## Rsc.Overallocated field

리소스가 특정 작업 또는 모든 작업에 대해 정상 작업 용량 내에서 완료할 수 있는 것보다 더 많은 작업이 할당되었는지 여부를 나타냅니다.

```csharp
public static readonly Key<NullableBool, RscKey> Overallocated;
```

## 예제

Tsk.IsOverallocated, Tsk.HasOverallocatedResource 를 읽는 방법을 보여줍니다,

```csharp
// Rsc.Overallocated 및 Asn.Overallocated 속성.
var project = new Project();

var task1 = project.RootTask.Children.Add("Task1");
var task2 = project.RootTask.Children.Add("Task2");

var resource1 = project.Resources.Add("Resource1");
var resource2 = project.Resources.Add("Resource2");

project.CalculationMode = CalculationMode.None;
task1.Set(Tsk.Type, TaskType.FixedDuration);
var assignment11 = project.ResourceAssignments.Add(task1, resource1);
assignment11.Set(Asn.Work, project.GetDuration(9, TimeUnitType.Hour));
assignment11.Set(Asn.Start, task1.Get(Tsk.Start));
assignment11.Set(Asn.Finish, task1.Get(Tsk.Start).AddHours(9));
task1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task1.Set(Tsk.Work, project.GetDuration(9, TimeUnitType.Hour));
var assignment21 = project.ResourceAssignments.Add(task2, resource1);
var assignment22 = project.ResourceAssignments.Add(task2, resource2);

assignment21.Set(Asn.Work, project.GetDuration(1, TimeUnitType.Hour));

project.CalculationMode = CalculationMode.Automatic;
project.Recalculate();

Console.WriteLine("Task1: Is Overallocated: " + task1.Get(Tsk.IsOverallocated));
Console.WriteLine("Task2: Is Overallocated: " + task2.Get(Tsk.IsOverallocated));

Console.WriteLine("Task1: Has Overallocated Resource: " + task1.Get(Tsk.HasOverallocatedResource));
Console.WriteLine("Task2: Has Overallocated Resource: " + task2.Get(Tsk.HasOverallocatedResource));

Console.WriteLine("Resource1: Is Overallocated: " + resource1.Get(Rsc.Overallocated));
Console.WriteLine("Resource2: Is Overallocated: " + resource2.Get(Rsc.Overallocated));

Console.WriteLine("Assignment11: Is Overallocated: " + assignment11.Get(Asn.Overallocated));
Console.WriteLine("Assignment21: Is Overallocated: " + assignment21.Get(Asn.Overallocated));
Console.WriteLine("Assignment22: Is Overallocated: " + assignment22.Get(Asn.Overallocated));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


