---
title: "Tsk.NotesRTF"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。RTF 格式的文本备注。仅支持 MPP 格式"
type: docs
weight: 820
url: /zh/net/aspose.tasks/tsk/notesrtf/
---
## Tsk.NotesRTF field

RTF 格式的文本备注。仅支持 MPP 格式。

```csharp
public static readonly Key<string, TaskKey> NotesRTF;
```

## 示例

展示如何读取/写入 Tsk.NotesRTF 属性。

```csharp
var project = new Project();

            var task = project.RootTask.Children.Add("Task");

            const string rtf = @"{\rtf1\ansi\ansicpg1252\deff0\deflang1033{\fonttbl{\f0\fnil\fcharset134 SimSun;}{\f1\fnil\fcharset0 Calibri;}}
{\*\generator Msftedit 5.41.21.2510;}\viewkind4\uc1\pard\sa200\sl276\slmult1\lang9\f0\fs22\'d4\'e7\'c9\'cf\'ba\'c3\f1\par
}
 "; // 早上好

            task.Set(Tsk.NotesRTF, rtf);

            Console.WriteLine("Notes RTF: " + task.Get(Tsk.NotesRTF));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


