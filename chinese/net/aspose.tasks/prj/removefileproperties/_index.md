---
title: "Prj.RemoveFileProperties"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定在保存时是否会删除所有文件属性"
type: docs
weight: 600
url: /zh/net/aspose.tasks/prj/removefileproperties/
---
## Prj.RemoveFileProperties field

确定在保存时是否会删除所有文件属性。

```csharp
public static readonly Key<NullableBool, PrjKey> RemoveFileProperties;
```

## 示例

展示如何读取/写入 Prj.RemoveFileProperties 属性。

```csharp
var project = new Project();

project.Set(Prj.RemoveFileProperties, true);

Console.WriteLine("Remove File Properties: " + project.Get(Prj.RemoveFileProperties));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


