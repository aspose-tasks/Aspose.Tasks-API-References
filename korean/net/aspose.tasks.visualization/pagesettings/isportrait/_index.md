---
title: "PageSettings.IsPortrait"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PageSettings 속성. 페이지 방향이 세로인지 여부를 나타내는 값을 가져오거나 설정합니다. 페이지 방향이 가로인 경우 false를 반환합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks.visualization/pagesettings/isportrait/
---
## PageSettings.IsPortrait property

페이지 방향이 세로인지 여부를 나타내는 값을 가져오거나 설정합니다; 페이지 방향이 가로이면 false를 반환합니다.

```csharp
public bool IsPortrait { get; set; }
```

## 비고

SaveOptions.PageSize == Visualization.PageSize.DefinedInView인 경우 렌더링 중에 적용됩니다.

## 예제

&lt;see cref=\"Aspose.Tasks.Visualization.PageSettings\" /&gt;와 작업하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 설정을 가져옵니다
var settings = project.DefaultView.PageInfo.PageSettings;
// 몇몇 속성을 조정해 봅시다
// 페이지 방향이 세로인지 여부를 나타내는 값을 설정합니다; 페이지 방향이 가로이면 false를 반환합니다.
settings.IsPortrait = true;
// 인쇄할 너비 방향 페이지 수를 설정합니다.
settings.PagesInWidth = 5;
// 인쇄할 높이 방향 페이지 수를 설정합니다.
settings.PagesInHeight = 7;
// 인쇄를 조정할 정상 크기의 백분율을 설정합니다.
settings.PercentOfNormalSize = 200;
// 용지 크기를 설정합니다. <see cref=\"T:Aspose.Tasks.Visualization.PrinterPaperSize\" /> 열거형의 값 중 하나일 수 있습니다.
settings.PaperSize = PrinterPaperSize.PaperB4;
// 인쇄할 첫 페이지 번호를 설정합니다.
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

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

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


