---
title: "Asn.Resource"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。分配给任务的资源"
type: docs
weight: 470
url: /zh/net/aspose.tasks/asn/resource/
---
## Asn.Resource field

分配给任务的资源。

```csharp
public static readonly Key<Resource, AsnKey> Resource;
```

## 示例

展示如何读取 Asn.Task 和 Asn.Resource 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assigned Task Name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
Console.WriteLine("Assigned Resource Name: " + assignment.Get(Asn.Resource).Get(Rsc.Name));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Resource](../../resource/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


