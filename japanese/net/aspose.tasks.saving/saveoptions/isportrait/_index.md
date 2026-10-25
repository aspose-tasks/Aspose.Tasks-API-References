---
title: "SaveOptions.IsPortrait"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "SaveOptions プロパティ。ページの向きが縦向きかどうかを示す値を取得または設定します。ページの向きが横向きの場合は false を返します"
type: docs
weight: 70
url: /ja/net/aspose.tasks.saving/saveoptions/isportrait/
---
## SaveOptions.IsPortrait property

ページの向きが縦向きかどうかを示す値を取得または設定します。ページの向きが横向きの場合は false を返します。

```csharp
public bool IsPortrait { get; set; }
```

## 備考

SaveOptions.PageSize が Visualization.PageSize.DefinedInView の場合は適用されません。この場合は代わりに View.PageInfo.PageSettings.IsPortrait が使用されます。SaveOptions.CustomPageSize が設定されている場合も適用されません。

## 例

View 設定または SaveOptions を使用してページサイズと向きを指定する方法を示します。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// この場合、ページサイズと向きは view.PageInfo.PageSettings.PaperSize と view.PageInfo.PageSettings.IsPortrait プロパティから適用されます。
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// この場合、ページサイズと向きは SaveOptions のプロパティから適用されます。
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// この場合、ページサイズは SaveOptions.CustomPageSize から適用されます。IsPortrait プロパティは考慮されません。
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### 関連項目

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


