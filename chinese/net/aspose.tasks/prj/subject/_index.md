---
title: "Prj.Subject"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。项目的主题"
type: docs
weight: 700
url: /zh/net/aspose.tasks/prj/subject/
---
## Prj.Subject field

项目的主题。

```csharp
public static readonly Key<string, PrjKey> Subject;
```

## 示例

展示如何读取/写入 Prj.Subject 属性。

```csharp
var project = new Project();

project.Set(Prj.Subject, "Subject");

Console.WriteLine("Subject: " + project.Get(Prj.Subject));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


