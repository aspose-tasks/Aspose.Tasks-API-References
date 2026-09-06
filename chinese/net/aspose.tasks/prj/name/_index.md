---
title: "Prj.Name"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。项目的名称"
type: docs
weight: 540
url: /zh/net/aspose.tasks/prj/name/
---
## Prj.Name field

项目的名称。

```csharp
public static readonly Key<string, PrjKey> Name;
```

## 示例

展示如何读取/写入项目名称。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

project.Set(Prj.Name, "Custom Project Name");

Console.WriteLine("Project name: " + project.Get(Prj.Name));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


