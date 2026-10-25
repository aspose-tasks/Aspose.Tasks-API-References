---
title: "Asn.PeakUnits"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 작업에 대해 리소스가 할당되는 최대 단위 수"
type: docs
weight: 390
url: /ko/net/aspose.tasks/asn/peakunits/
---
## Asn.PeakUnits field

리소스가 작업에 할당되는 최대 단위 수.

```csharp
public static readonly Key<double, AsnKey> PeakUnits;
```

## 예제

공통 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2020, 4, 9, 8, 0, 0));
assignment.Set(Asn.Work, project.GetWork(1));
assignment.Set(Asn.Finish, new DateTime(2020, 4, 9, 17, 0, 0));
assignment.Set(Asn.Units, 1);
assignment.Set(Asn.PeakUnits, 1);

Console.WriteLine("Start: " + assignment.Get(Asn.Start));
Console.WriteLine("Work: " + assignment.Get(Asn.Work));
Console.WriteLine("Finish: " + assignment.Get(Asn.Finish));
Console.WriteLine("Units: " + assignment.Get(Asn.Units));
Console.WriteLine("Peak Units: " + assignment.Get(Asn.PeakUnits));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


