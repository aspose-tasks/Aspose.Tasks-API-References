---
title: "Asn.Milestone"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。确定分配是否为里程碑"
type: docs
weight: 330
url: /zh/net/aspose.tasks/asn/milestone/
---
## Asn.Milestone field

确定任务是否为里程碑。

```csharp
public static readonly Key<bool, AsnKey> Milestone;
```

## 示例

展示如何读取 Asn.Milestone 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Milestone: " + assignment.Get(Asn.Milestone));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


