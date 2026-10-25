---
title: "Prj.AdminProject"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定项目是否为行政项目"
type: docs
weight: 20
url: /zh/net/aspose.tasks/prj/adminproject/
---
## Prj.AdminProject field

确定项目是否为管理项目。

```csharp
public static readonly Key<NullableBool, PrjKey> AdminProject;
```

## 示例

展示如何读取/写入 Prj.AdminProject 属性。

```csharp
var project = new Project();

project.Set(Prj.AdminProject, true);

Console.WriteLine("Admin Project: " + project.Get(Prj.AdminProject));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


