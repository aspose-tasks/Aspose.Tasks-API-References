---
title: "열거형 TextItemType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.TextItemType 열거형. 텍스트 스타일을 변경할 항목 유형"
type: docs
weight: 3410
url: /ko/net/aspose.tasks.visualization/textitemtype/
---
## TextItemType enumeration

텍스트 스타일을 변경할 항목 유형입니다.

```csharp
public enum TextItemType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| RowColumnTitles | `0` | 행 및 열 제목. |
| CriticalTasks | `1` | 중요 작업. |
| NoncriticalTasks | `2` | 비중요 작업. |
| MilestoneTasks | `3` | 마일스톤 작업. |
| InactiveTasks | `4` | 비활성 작업. |
| SummaryTasks | `5` | 요약 작업. |
| AssignmentRow | `6` | 할당 행. |
| TopTimescaleTier | `7` | 상위 시간축 계층. |
| BottomTimescaleTier | `8` | 하위 시간축 계층. |
| MiddleTimescaleTier | `9` | 중간 시간축 계층. |
| Resources | `10` | 리소스 시트. |
| OverallocatedResources | `11` | 과다 할당된 리소스. |
| TaskFilterHighlight | `12` | 작업 필터 강조 텍스트 항목. |
| BarTextBottom | `13` | 바 텍스트 하단 텍스트 항목. |
| BarTextInside | `14` | 바 텍스트 내부 텍스트 항목. |
| BarTextLeft | `15` | 바 텍스트 왼쪽 텍스트 항목. |
| BarTextRight | `16` | 바 텍스트 오른쪽 텍스트 항목. |
| BarTextTop | `17` | 바 텍스트 상단 텍스트 항목. |
| MarkedTasks | `18` | 표시된 작업 텍스트 항목. |
| ProjectSummary | `19` | 프로젝트 요약 작업 텍스트 항목. |
| ExternalTasks | `20` | 외부 작업 텍스트 항목. |
| Allocated | `21` | 할당된 텍스트 항목. |
| ChangedCells | `22` | 변경된 셀. |

## 예제

텍스트 항목 유형을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Italic | FontStyles.Bold)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### 또 보기

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


