---
title: "Asn.UpdateNeeded"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。确定分配给任务的资源是否需要根据任务状态进行更新"
type: docs
weight: 580
url: /zh/net/aspose.tasks/asn/updateneeded/
---
## Asn.UpdateNeeded field

确定分配给任务的资源是否需要根据任务状态进行更新。

```csharp
public static readonly Key<bool, AsnKey> UpdateNeeded;
```

## 示例

展示如何读取/写入 Asn.UpdateNeeded 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.UpdateNeeded, true);

Console.WriteLine("Update Needed: " + assignment.Get(Asn.UpdateNeeded));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


