---
title: "Prj.Title"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。项目的标题"
type: docs
weight: 750
url: /zh/net/aspose.tasks/prj/title/
---
## Prj.Title field

项目的标题。

```csharp
public static readonly Key<string, PrjKey> Title;
```

## 示例

展示如何读取/写入 Prj.Title 属性。

```csharp
var project = new Project();

project.Set(Prj.Title, "MS Project");

Console.WriteLine("Title: " + project.Get(Prj.Title));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


