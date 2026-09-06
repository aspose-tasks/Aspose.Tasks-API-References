---
title: "Asn.HasFixedRateUnits"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。确定单位是否具有固定费率"
type: docs
weight: 270
url: /zh/net/aspose.tasks/asn/hasfixedrateunits/
---
## Asn.HasFixedRateUnits field

确定单位是否具有固定费率。

```csharp
public static readonly Key<bool, AsnKey> HasFixedRateUnits;
```

## 示例

展示如何读取/写入 Asn.HasFixedRateUnits 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.HasFixedRateUnits, true);

Console.WriteLine("Has Fixed Rate Units: " + assignment.Get(Asn.HasFixedRateUnits));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


