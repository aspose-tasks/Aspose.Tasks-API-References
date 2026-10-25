---
title: "Rsc.Workgroup"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源所属工作组的类型"
type: docs
weight: 700
url: /zh/net/aspose.tasks/rsc/workgroup/
---
## Rsc.Workgroup field

资源所属工作组的类型。

```csharp
public static readonly Key<WorkGroupType, RscKey> Workgroup;
```

## 示例

展示如何读取/写入 Rsc.Workgroup 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Workgroup, WorkGroupType.Email);

Console.WriteLine("Workgroup: " + resource.Get(Rsc.Workgroup));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [WorkGroupType](../../workgrouptype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


