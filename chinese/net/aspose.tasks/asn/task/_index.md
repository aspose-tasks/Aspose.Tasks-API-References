---
title: "Asn.Task"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。资源被分配到的任务"
type: docs
weight: 550
url: /zh/net/aspose.tasks/asn/task/
---
## Asn.Task field

资源被分配到的任务。

```csharp
public static readonly Key<Task, AsnKey> Task;
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
* class [Task](../../task/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


