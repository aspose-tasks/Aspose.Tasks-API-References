---
title: "Asn.Delay"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。分配的延迟"
type: docs
weight: 230
url: /zh/net/aspose.tasks/asn/delay/
---
## Asn.Delay field

任务的延迟。

```csharp
public static readonly Key<Duration, AsnKey> Delay;
```

## 示例

展示如何读取/写入 Asn.Delay 和 Asn.LevelingDelay 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Delay, project.GetDuration(0, TimeUnitType.Day));

Console.WriteLine("Delay: " + assignment.Get(Asn.Delay));
Console.WriteLine("Leveling Delay: " + assignment.Get(Asn.LevelingDelay));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


