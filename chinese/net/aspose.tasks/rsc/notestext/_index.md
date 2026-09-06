---
title: "Rsc.NotesText"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。从 RTF 数据中提取的笔记纯文本"
type: docs
weight: 480
url: /zh/net/aspose.tasks/rsc/notestext/
---
## Rsc.NotesText field

从 RTF 数据中提取的备注纯文本。

```csharp
public static readonly Key<string, RscKey> NotesText;
```

## 示例

展示如何读取/写入 Rsc.NotesText 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.NotesText, "Resource Notes");

Console.WriteLine("Notes text: " + resource.Get(Rsc.NotesText));
Console.WriteLine("Notes RTF: " + resource.Get(Rsc.NotesRTF));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


