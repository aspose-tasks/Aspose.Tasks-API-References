---
title: "Asn.FixedMaterial"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。确定已分配的材料资源的消耗是否以单一固定量发生"
type: docs
weight: 260
url: /zh/net/aspose.tasks/asn/fixedmaterial/
---
## Asn.FixedMaterial field

确定已分配的材料资源消耗是否以单一、固定数量进行。

```csharp
public static readonly Key<bool, AsnKey> FixedMaterial;
```

## 示例

展示如何读取/写入 Asn.FixedMaterial 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.FixedMaterial, true);

Console.WriteLine("Fixed Material: " + assignment.Get(Asn.FixedMaterial));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


