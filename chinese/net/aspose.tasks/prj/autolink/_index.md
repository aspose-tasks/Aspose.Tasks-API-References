---
title: "Prj.Autolink"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定插入或移动的任务是否自动链接"
type: docs
weight: 70
url: /zh/net/aspose.tasks/prj/autolink/
---
## Prj.Autolink field

确定插入或移动的任务是否自动链接。

```csharp
public static readonly Key<NullableBool, PrjKey> Autolink;
```

## 示例

展示如何读取/写入 Prj.Autolink 属性。

```csharp
var project = new Project();

project.Set(Prj.Autolink, true);

Console.WriteLine("Autolink: " + project.Get(Prj.Autolink));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


