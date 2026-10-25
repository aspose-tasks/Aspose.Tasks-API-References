---
title: "Tsk.NotesText"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。从 RTF 数据中提取的笔记纯文本。"
type: docs
weight: 830
url: /zh/net/aspose.tasks/tsk/notestext/
---
## Tsk.NotesText field

从 RTF 数据中提取的备注纯文本。

```csharp
public static readonly Key<string, TaskKey> NotesText;
```

## 示例

展示如何读取/写入 Tsk.NotesText 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.NotesText, "Notes");

Console.WriteLine("Notes Text: " + task.Get(Tsk.NotesText));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


