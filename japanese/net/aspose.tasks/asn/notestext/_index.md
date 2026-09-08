---
title: "Asn.NotesText"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Asn フィールド。RTF データから抽出されたノートのプレーンテキスト"
type: docs
weight: 350
url: /ja/net/aspose.tasks/asn/notestext/
---
## Asn.NotesText field

ノートのプレーンテキスト（RTF データから抽出）。

```csharp
public static readonly Key<string, AsnKey> NotesText;
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


