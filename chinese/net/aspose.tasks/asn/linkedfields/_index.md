---
title: "Asn.LinkedFields"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。确定项目是否链接到另一个 OLE 对象"
type: docs
weight: 320
url: /zh/net/aspose.tasks/asn/linkedfields/
---
## Asn.LinkedFields field

确定项目是否链接到其他 OLE 对象。

```csharp
public static readonly Key<bool, AsnKey> LinkedFields;
```

## 示例

展示如何读取 Asn.LinkedFields 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Linked Fields: " + assignment.Get(Asn.LinkedFields));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


