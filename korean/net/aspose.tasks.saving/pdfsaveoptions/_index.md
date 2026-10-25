---
title: "클래스 PdfSaveOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.PdfSaveOptions 클래스. 프로젝트 페이지를 PDF로 렌더링할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 2130
url: /ko/net/aspose.tasks.saving/pdfsaveoptions/
---
## PdfSaveOptions class

프로젝트 페이지를 PDF로 렌더링할 때 추가 옵션을 지정할 수 있습니다.

```csharp
public class PdfSaveOptions : SaveOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | `PdfSaveOptions` 클래스의 새 인스턴스를 초기화합니다. 이 인스턴스는 [`PDF`](../savefileformat/) 형식으로 문서를 저장하는 데 사용할 수 있습니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | 프로젝트 보기에서 표시되는 [`BarStyle`](../../aspose.tasks.visualization/barstyle/) 클래스 인스턴스 목록을 가져오거나 설정합니다. |
| [Compliance](../../aspose.tasks.saving/pdfsaveoptions/compliance/) { get; set; } | 생성된 PDF 문서의 원하는 호환성 수준을 가져오거나 설정합니다. 기본값은 Pdf15입니다. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | 맞춤 페이지 크기를 포인트 단위로 가져오거나 설정합니다 (1 포인트 = 1/72 인치). |
| [DigitalSignatureDetails](../../aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/) { get; set; } | 디지털 서명 세부 정보를 가져오거나 설정합니다. 설정하지 않으면 서명이 수행되지 않습니다. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | 비작업 시간을 그릴지 여부를 나타내는 값을 가져오거나 설정합니다 (기본값은 TRUE). |
| [EncryptionDetails](../../aspose.tasks.saving/pdfsaveoptions/encryptiondetails/) { get; set; } | 암호화 세부 정보를 가져오거나 설정합니다. 설정하지 않으면 암호화가 수행되지 않습니다. |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | 렌더링을 종료할 날짜를 가져오거나 설정합니다. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | 행 높이를 내용에 맞게 늘릴지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [FontSettings](../../aspose.tasks.saving/pdfsaveoptions/fontsettings/) { get; } | 프로젝트 보기 렌더링 시 사용되는 글꼴 설정을 지정합니다. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | 프로젝트 뷰에 표시되는 [`Gridline`](../../aspose.tasks.visualization/gridline/) 목록을 가져오거나 설정합니다. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | 페이지 방향이 세로인지 여부를 나타내는 값을 가져오거나 설정합니다; 페이지 방향이 가로이면 false를 반환합니다. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | 범례를 렌더링하는 방법을 정의하는 값을 가져오거나 설정합니다. 기본값은 LegendDrawingOptions.OnEveryPage입니다. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | 페이지 범례에 렌더링될 막대를 정의하는 PageLegendItem 배열을 가져오거나 설정합니다. null인 경우 기본 항목이 렌더링됩니다. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | 중요 작업을 빨간색으로 표시할지 여부를 나타내는 값을 가져오거나 설정합니다 (기본값은 FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | 비작업 시간 색상을 가져오거나 설정합니다. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | 프로젝트 페이지 수를 가져오거나 설정합니다. |
| [Pages](../../aspose.tasks.saving/pdfsaveoptions/pages/) { get; set; } | 프로젝트 레이아웃을 별도 파일로 저장할 때 저장할 페이지 번호 목록을 가져오거나 설정합니다. 이 목록이 비어 있으면 모든 페이지가 저장됩니다. |
| [PageSavingCallback](../../aspose.tasks.saving/pdfsaveoptions/pagesavingcallback/) { get; set; } | 각 렌더링된 페이지에 대한 출력 스트림을 가져오는 데 사용되는 사용자 정의 콜백을 가져오거나 설정합니다. [`SaveToSeparateFiles`](./savetoseparatefiles/) 옵션을 사용할 때 적용됩니다. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | 렌더링될 페이지 크기를 가져오거나 설정합니다 (기본값은 PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | 문서가 저장될 [`PresentationFormat`](../saveoptions/presentationformat/)을 가져오거나 설정합니다. |
| [ReduceFooterGap](../../aspose.tasks.saving/pdfsaveoptions/reducefootergap/) { get; set; } | 마지막 작업과 푸터 사이의 간격을 줄일지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | 프로젝트가 그래픽 형식으로 저장될 때 단일 페이지로 렌더링할지 여부를 나타내는 값을 가져오거나 설정합니다. 렌더링된 프로젝트가 한 페이지에 맞도록 페이지 크기가 조정됩니다. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | 요약 작업 막대에 하위 작업을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. 하위 작업의 경우, Rollup 필드는 하위 작업 Gantt 막대의 정보가 요약 작업 막대로 집계될지 여부를 나타냅니다. 요약 작업의 경우, Rollup 필드는 요약 작업 막대가 집계된 막대를 표시할지 여부를 나타냅니다. 하위 작업을 집계하려면 요약 작업에 대한 Rollup 필드를 Yes로 설정해야 합니다. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 이 저장 옵션 개체가 사용될 경우 문서가 저장되는 형식을 가져오거나 설정합니다. |
| [SaveToSeparateFiles](../../aspose.tasks.saving/pdfsaveoptions/savetoseparatefiles/) { get; set; } | 프로젝트 페이지를 별도 파일로 저장할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | 렌더링을 시작할 날짜를 가져오거나 설정합니다. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | 작업 링크 렌더링의 일부 측면을 사용자 지정하는 데 사용할 수 있는 콜백을 가져오거나 설정합니다. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 간트 차트 및 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 가져오거나 설정합니다. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 간트, 작업 시트 및 작업 사용 차트에 렌더링된 작업을 필터링하는 데 사용되는 조건을 가져오거나 설정합니다. |
| [TextCompression](../../aspose.tasks.saving/pdfsaveoptions/textcompression/) { get; set; } | 이미지를 제외한 모든 콘텐츠 스트림에 사용할 압축 유형을 가져오거나 설정합니다. 기본값은 Flate입니다. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | 프로젝트 뷰 렌더링 중에 적용되는 텍스트 스타일 목록을 가져오거나 설정합니다. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | 프로젝트를 그래픽 형식으로 저장할 때 타임스케일(있는 경우)이 렌더링되는 방식을 제어하는 ​​[`Timescale`](../saveoptions/timescale/) 값을 가져오거나 설정합니다. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | 타임스케일의 오른쪽 끝을 페이지 끝에 맞추는 방식을 정의하는 동작을 가져오거나 설정합니다. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Gantt 차트를 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | 렌더링할 뷰 열 목록을 가져오거나 설정합니다 ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). 설정되지 않으면 작업 ID, 작업 이름, 시작 및 종료만 렌더링됩니다. View와 [`ViewSettings`](../saveoptions/viewsettings/) 속성이 모두 설정된 경우, View의 열이 ViewSettings의 열을 우선합니다. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | 렌더링할 뷰 ([`View`](../saveoptions/view/))를 가져오거나 설정합니다. 이 옵션을 사용하여 PDF, HTML 또는 이미지 형식으로 저장될 뷰를 명시적으로 지정할 수 있습니다. 이 속성이 설정되면 프로젝트 저장 시 [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) 속성이 무시됩니다. 뷰는 다음 화면 중 하나여야 합니다 (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

## 예제

프로젝트의 선택된 페이지를 PDF 파일로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// 내보낼 수 있는 페이지 수를 확인해 봅시다
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### 또 보기

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


