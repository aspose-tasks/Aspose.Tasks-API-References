---
title: "Asn.Summary"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。确定任务是否为汇总任务"
type: docs
weight: 530
url: /zh/net/aspose.tasks/asn/summary/
---
## Asn.Summary field

确定任务是否为汇总任务。

```csharp
public static readonly Key<bool, AsnKey> Summary;
```

## 示例

展示如何读取 Asn.Summary 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Summary, true);

Console.WriteLine("Summary: " + assignment.Get(Asn.Summary));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


