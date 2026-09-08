---
title: "Asn.NotesRTF"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Asn フィールド。RTF 形式のテキストノート。MPP 形式のみサポートされます"
type: docs
weight: 340
url: /ja/net/aspose.tasks/asn/notesrtf/
---
## Asn.NotesRTF field

RTF 形式のテキストノート。MPP 形式のみサポートされます。

```csharp
public static readonly Key<string, AsnKey> NotesRTF;
```

## 例

リソース割り当てノートの取得/設定方法を示します。

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// リソース割り当てを作成する
var assn = project.ResourceAssignments.Add(task, rsc);

// リソース割り当てノートを設定する
assn.Set(Asn.NotesText, "Newly added assignment");

Console.WriteLine("Notes text: " + assn.Get(Asn.NotesText));
Console.WriteLine("Notes RTF: " + assn.Get(Asn.NotesRTF));
```

### 関連項目

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


