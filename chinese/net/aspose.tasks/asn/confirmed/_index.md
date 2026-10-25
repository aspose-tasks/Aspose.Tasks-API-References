---
title: "Asn.Confirmed"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。确定资源是否已接受其所有分配"
type: docs
weight: 170
url: /zh/net/aspose.tasks/asn/confirmed/
---
## Asn.Confirmed field

确定资源是否已接受其所有任务。

```csharp
public static readonly Key<bool, AsnKey> Confirmed;
```

## 示例

展示如何读取/写入 Asn.Confirmed 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Confirmed, true);

Console.WriteLine("Confirmed: " + assignment.Get(Asn.Confirmed));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


