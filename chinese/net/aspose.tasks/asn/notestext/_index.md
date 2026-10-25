---
title: "Asn.NotesText"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。从 RTF 数据中提取的笔记纯文本"
type: docs
weight: 350
url: /zh/net/aspose.tasks/asn/notestext/
---
## Asn.NotesText field

从 RTF 数据中提取的备注纯文本。

```csharp
public static readonly Key<string, AsnKey> NotesText;
```

## 示例

展示如何获取/设置资源任务备注。

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// 创建资源任务
var assn = project.ResourceAssignments.Add(task, rsc);

// 设置资源任务备注 
assn.Set(Asn.NotesText, "Newly added assignment");

Console.WriteLine("Notes text: " + assn.Get(Asn.NotesText));
Console.WriteLine("Notes RTF: " + assn.Get(Asn.NotesRTF));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


