---
title: "Asn.Created"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。创建任务的日期"
type: docs
weight: 210
url: /zh/net/aspose.tasks/asn/created/
---
## Asn.Created field

任务创建的日期。

```csharp
public static readonly Key<DateTime, AsnKey> Created;
```

## 示例

展示如何读取/写入 Asn.Created 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Created, new DateTime(2020, 4, 9, 8, 0, 0));

Console.WriteLine("Created: " + assignment.Get(Asn.Created));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


