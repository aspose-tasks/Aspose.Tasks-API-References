---
title: "Asn.RegularWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。为分配安排的非加班工作量"
type: docs
weight: 420
url: /zh/net/aspose.tasks/asn/regularwork/
---
## Asn.RegularWork field

分配的非加班工作量。

```csharp
public static readonly Key<Duration, AsnKey> RegularWork;
```

## 示例

展示如何读取/写入 Asn.RegularWork 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + assignment.Get(Asn.RegularWork));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


