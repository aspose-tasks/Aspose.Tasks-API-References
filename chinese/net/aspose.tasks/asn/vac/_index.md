---
title: "Asn.VAC"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。基准成本与总成本之间的差额"
type: docs
weight: 590
url: /zh/net/aspose.tasks/asn/vac/
---
## Asn.VAC field

基线成本与总成本之间的差额。

```csharp
public static readonly Key<double, AsnKey> VAC;
```

## 示例

展示如何读取 Asn.VAC 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.VAC, 10);

Console.WriteLine("VAC: " + assignment.Get(Asn.VAC));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


