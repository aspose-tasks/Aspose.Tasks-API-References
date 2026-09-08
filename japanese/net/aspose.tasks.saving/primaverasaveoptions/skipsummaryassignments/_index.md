---
title: "PrimaveraSaveOptions.SkipSummaryAssignments"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "PrimaveraSaveOptions プロパティ。エクスポート時にリソースのサマリ タスクへの割り当てをスキップするかどうかを示す値を取得または設定します"
type: docs
weight: 60
url: /ja/net/aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/
---
## PrimaveraSaveOptions.SkipSummaryAssignments property

エクスポート時にリソースのサマリータスクへの割り当てをスキップするかどうかを示す値を取得または設定します。

```csharp
public bool SkipSummaryAssignments { get; set; }
```

## 備考

Primavera ソフトウェアはリソースをサマリー（WBS）タスクに割り当てることをサポートしていません。そのため、これらの割り当てをエクスポートすると、Primavera のモデルに従って無効なファイルになる可能性があります。true の場合、サマリータスクへの割り当てはエクスポート時にスキップされます。false（デフォルト値）の場合、エクスポート中にサマリータスクへの割り当てが検出されると例外がスローされます。

## 例

SkipSummaryAssignments フラグの使用方法を示します。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var resource = project.Resources.Add("Resource");

var summaryTask = project.RootTask.Children.Add("Summary");
summaryTask.Children.Add("Task");

// Primavera はリソースをサマリータスクに割り当てることをサポートしていません。
// そのため、これらの割り当てを Primavera 形式でエクスポートすると、Primavera にインポートできないファイルになる可能性があります。
var assignment = project.ResourceAssignments.Add(summaryTask, resource);

var options = new PrimaveraXmlSaveOptions();
options.SkipSummaryAssignments = true;
project.Save(OutDir + "UseSkipSummaryAssignments_out.xml", options);
```

### 関連項目

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


