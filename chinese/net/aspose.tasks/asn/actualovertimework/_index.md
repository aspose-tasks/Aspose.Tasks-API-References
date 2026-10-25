---
title: "Asn.ActualOvertimeWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。实际在任务上产生的加班工作量"
type: docs
weight: 40
url: /zh/net/aspose.tasks/asn/actualovertimework/
---
## Asn.ActualOvertimeWork field

分配的实际加班工作量。

```csharp
public static readonly Key<Duration, AsnKey> ActualOvertimeWork;
```

## 示例

展示如何读取/写入实际属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2000, 1, 3, 8, 0, 0));
assignment.Set(Asn.Work, project.GetWork(8));
assignment.Set(Asn.Finish, new DateTime(2000, 1, 3, 17, 0, 0));
assignment.Set(Asn.ActualStart, new DateTime(2000, 1, 3, 8, 0, 0));
assignment.Set(Asn.ActualWork, project.GetDuration(8, TimeUnitType.Hour));
assignment.Set(Asn.ActualWorkProtected, project.GetDuration(8, TimeUnitType.Hour));
assignment.Set(Asn.ActualFinish, new DateTime(2000, 1, 3, 17, 0, 0));
assignment.Set(Asn.ActualOvertimeWork, project.GetWork(1));
assignment.Set(Asn.ActualOvertimeCost, 1m);
assignment.Set(Asn.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Start: " + assignment.Get(Asn.Start));
Console.WriteLine("Work: " + assignment.Get(Asn.Work));
Console.WriteLine("Finish: " + assignment.Get(Asn.Finish));
Console.WriteLine("Actual Start: " + assignment.Get(Asn.ActualStart));
Console.WriteLine("Actual Work: " + assignment.Get(Asn.ActualWork));
Console.WriteLine("Actual Work Protected: " + assignment.Get(Asn.ActualWorkProtected));
Console.WriteLine("Actual Finish: " + assignment.Get(Asn.ActualFinish));
Console.WriteLine("Actual Overtime Work: " + assignment.Get(Asn.ActualOvertimeWork));
Console.WriteLine("Actual Overtime Cost: " + assignment.Get(Asn.ActualOvertimeCost));
Console.WriteLine("Actual Overtime Work Protected: " + assignment.Get(Asn.ActualOvertimeWorkProtected));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


