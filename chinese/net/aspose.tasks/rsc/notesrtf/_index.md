---
title: "Rsc.NotesRTF"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。RTF 格式的文本备注。仅支持 MPP 格式"
type: docs
weight: 470
url: /zh/net/aspose.tasks/rsc/notesrtf/
---
## Rsc.NotesRTF field

RTF 格式的文本备注。仅支持 MPP 格式。

```csharp
public static readonly Key<string, RscKey> NotesRTF;
```

## 示例

展示如何读取/写入 Rsc.NotesRTF 属性。

```csharp
var project = new Project();

            var resource = project.Resources.Add("Resource");

            const string RTF = @"{\rtf1\ansi\ansicpg1252\deff0\deflang1033{\fonttbl{\f0\fnil\fcharset134 SimSun;}{\f1\fnil\fcharset0 Calibri;}}
{\*\generator Msftedit 5.41.21.2510;}\viewkind4\uc1\pard\sa200\sl276\slmult1\lang9\f0\fs22\'d4\'e7\'c9\'cf\'ba\'c3\f1\par
}
 "; // 早上好

            resource.Set(Rsc.NotesRTF, RTF);

            Console.WriteLine("Notes RTF: " + resource.Get(Rsc.NotesRTF));
            Console.WriteLine("Notes text: " + resource.Get(Rsc.NotesText));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


