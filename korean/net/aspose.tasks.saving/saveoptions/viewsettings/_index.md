---
title: "SaveOptions.ViewSettings"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 렌더링할 View를 가져오거나 설정합니다. 이 옵션을 사용하여 PDF, HTML 또는 Image 형식으로 저장될 뷰를 명시적으로 지정할 수 있습니다. 이 속성이 설정된 경우 프로젝트를 저장할 때 PresentationFormat 속성이 무시됩니다. View는 다음 화면 중 하나인 Screen, Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage 중에서 선택되어야 합니다."
type: docs
weight: 240
url: /ko/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

렌더링할 view ([`View`](../view/))를 가져오거나 설정합니다. 이 옵션을 사용하여 PDF, HTML 또는 Image 형식으로 저장될 뷰를 명시적으로 지정할 수 있습니다. 이 속성이 설정된 경우, 프로젝트를 저장할 때 [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) 속성이 무시됩니다. View는 다음 화면 중 하나인 (([`Screen`](../../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)에서 선택되어야 합니다.

```csharp
public View ViewSettings { get; set; }
```

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentException | set 메서드가 호출되고 지원되지 않는 Screen 속성 값을 가진 View 클래스 인스턴스가 제공될 때. |

## 예제

'SaveOptions.ViewSettings'를 사용하여 PDF로 렌더링될 뷰를 지정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);
Console.WriteLine("Page size specified in view settings: " + view.PageInfo.PageSettings.PaperSize);
Console.WriteLine("Page orientation: {0}", view.PageInfo.PageSettings.IsPortrait ? "Portrait" : "Landscape");

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.DefinedInView;
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

project.Save(OutDir + "SaveToPdfUsingSpecificView_out.pdf", saveOptions);
```

### 또 보기

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


