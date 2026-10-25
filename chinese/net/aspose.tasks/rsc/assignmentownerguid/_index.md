---
title: "Rsc.AssignmentOwnerGuid"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。分配所有者的 GUID"
type: docs
weight: 110
url: /zh/net/aspose.tasks/rsc/assignmentownerguid/
---
## Rsc.AssignmentOwnerGuid field

分配所有者的 GUID。

```csharp
public static readonly Key<string, RscKey> AssignmentOwnerGuid;
```

## 示例

展示如何读取/写入 Rsc.AssignmentOwnerGuid 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwnerGuid, "aad9ac22-9f06-4196-906b-916acebcc1c2");

Console.WriteLine("Assignment Owner Guid: " + resource.Get(Rsc.AssignmentOwnerGuid));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


