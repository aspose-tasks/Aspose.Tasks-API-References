---
title: "PageViewSettings.FirstColumnsCount"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PageViewSettings 속성. 모든 페이지에 인쇄될 첫 번째 열의 수를 가져오거나 설정합니다"
type: docs
weight: 20
url: /ko/net/aspose.tasks.visualization/pageviewsettings/firstcolumnscount/
---
## PageViewSettings.FirstColumnsCount property

모든 페이지에 인쇄될 첫 번째 열의 수를 가져오거나 설정합니다.

```csharp
public int FirstColumnsCount { get; set; }
```

## 예제

작업, 리소스, 할당 노트를 별도의 페이지에 인쇄하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Input.mpp");

// 모든 페이지에 인쇄될 첫 번째 열의 개수를 설정합니다.
project.DefaultView.PageInfo.PageViewSettings.FirstColumnsCount = 2;

// 노트를 인쇄할지 여부를 나타내는 값을 설정합니다.
project.DefaultView.PageInfo.PageViewSettings.PrintNotes = true;

// 인쇄 시 시간 눈금을 페이지 끝에 맞출지 여부를 나타내는 값을 설정합니다.
project.DefaultView.PageInfo.PageViewSettings.FitTimescaleToEndOfPage = true;

// 뷰의 모든 시트 열을 인쇄할지 여부를 나타내는 값을 설정합니다
project.DefaultView.PageInfo.PageViewSettings.PrintAllSheetColumns = true;

// 뷰의 빈 페이지를 인쇄할지 여부를 나타내는 값을 설정합니다
project.DefaultView.PageInfo.PageViewSettings.PrintBlankPages = false;

// 모든 페이지에 지정된 수의 첫 번째 열을 인쇄할지 여부를 나타내는 값을 설정합니다.
project.DefaultView.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

project.Save(OutDir + "ProjectWithComments_out.pdf", SaveFileFormat.Pdf);
```

### 또 보기

* class [PageViewSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pageviewsettings/)
* assembly [Aspose.Tasks](../../../)


