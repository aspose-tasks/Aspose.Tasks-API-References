---
title: "Asn.Uid"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。任务的唯一标识符。"
type: docs
weight: 560
url: /zh/net/aspose.tasks/asn/uid/
---
## Asn.Uid field

分配的唯一标识符。

```csharp
public static readonly Key<int, AsnKey> Uid;
```

## 示例

展示如何读取/写入 Asn.Uid 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Uid, 30);

Console.WriteLine("UID: " + assignment.Get(Asn.Uid));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


