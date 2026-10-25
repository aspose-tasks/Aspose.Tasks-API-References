---
title: "Prj.Guid"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。项目的 GUID"
type: docs
weight: 360
url: /zh/net/aspose.tasks/prj/guid/
---
## Prj.Guid field

项目的 GUID。

```csharp
public static readonly Key<Guid, PrjKey> Guid;
```

## 示例

展示如何读取/写入 Prj.Guid 属性。

```csharp
var project = new Project();

project.Set(Prj.Guid, new Guid("efcc0d63-d8e0-4a34-9f3e-9f973f50238a"));

Console.WriteLine("Guid: " + project.Get(Prj.Guid));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


