---
title: "Rsc.AssignmentOwner"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。分配所有者的名称"
type: docs
weight: 100
url: /zh/net/aspose.tasks/rsc/assignmentowner/
---
## Rsc.AssignmentOwner field

分配所有者的名称。

```csharp
public static readonly Key<string, RscKey> AssignmentOwner;
```

## 示例

展示如何读取/写入 Rsc.AssignmentOwner 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwner, "John");

Console.WriteLine("Assignment Owner: " + resource.Get(Rsc.AssignmentOwner));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


