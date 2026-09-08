---
title: "SaveOptions.IsPortrait"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 페이지 방향이 세로인지 여부를 나타내는 값을 가져오거나 설정합니다. 페이지 방향이 가로인 경우 false를 반환합니다."
type: docs
weight: 70
url: /ko/net/aspose.tasks.saving/saveoptions/isportrait/
---
## SaveOptions.IsPortrait property

페이지 방향이 세로인지 여부를 나타내는 값을 가져오거나 설정합니다; 페이지 방향이 가로이면 false를 반환합니다.

```csharp
public bool IsPortrait { get; set; }
```

## 비고

SaveOptions.PageSize == Visualization.PageSize.DefinedInView인 경우 적용되지 않습니다. 이 경우 View.PageInfo.PageSettings.IsPortrait가 대신 사용됩니다. SaveOptions.CustomPageSize가 설정된 경우에도 적용되지 않습니다.

## 예제

View 설정 또는 SaveOptions를 사용하여 페이지 크기와 방향을 지정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// 이 경우 페이지 크기와 방향은 view.PageInfo.PageSettings.PaperSize 및 view.PageInfo.PageSettings.IsPortrait 속성에서 적용됩니다.
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// 이 경우 페이지 크기와 방향은 SaveOptions의 속성에서 적용됩니다.
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// 이 경우 페이지 크기는 SaveOptions.CustomPageSize에서 적용됩니다. IsPortrait 속성은 고려되지 않습니다.
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### 또 보기

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


