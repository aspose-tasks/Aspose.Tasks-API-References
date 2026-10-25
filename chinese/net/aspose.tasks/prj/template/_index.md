---
title: "Prj.Template"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。项目模板"
type: docs
weight: 720
url: /zh/net/aspose.tasks/prj/template/
---
## Prj.Template field

项目模板。

```csharp
public static readonly Key<string, PrjKey> Template;
```

## 示例

展示如何读取/写入 Prj.Template 属性。

```csharp
var project = new Project();

project.Set(Prj.Template, "Custom Template");

Console.WriteLine("Template: " + project.Get(Prj.Template));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


