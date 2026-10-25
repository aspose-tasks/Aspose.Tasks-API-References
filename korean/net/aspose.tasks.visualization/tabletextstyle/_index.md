---
title: "클래스 TableTextStyle"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.TableTextStyle 클래스. 보기 테이블의 텍스트 스타일을 나타냅니다"
type: docs
weight: 3370
url: /ko/net/aspose.tasks.visualization/tabletextstyle/
---
## TableTextStyle class

보기 테이블의 텍스트 스타일을 나타냅니다.

```csharp
public class TableTextStyle : TextStyle
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [TableTextStyle](tabletextstyle/#constructor)(int) | `TableTextStyle` 클래스의 새 인스턴스를 초기화합니다. |
| [TableTextStyle](tabletextstyle/#constructor_1)(int, FontDescriptor) | 지정된 폰트를 사용하여 `TableTextStyle` 클래스의 새 인스턴스를 초기화합니다. |
| [TableTextStyle](tabletextstyle/#constructor_2)(int, FontStyles) | 기본 폰트 설정과 지정된 폰트 스타일을 사용하여 `TableTextStyle` 클래스의 새 인스턴스를 초기화합니다. |
| [TableTextStyle](tabletextstyle/#constructor_3)(int, float, FontStyles) | 지정된 폰트 크기와 폰트 스타일을 사용하여 `TableTextStyle` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | 텍스트 스타일의 배경 색을 가져오거나 설정합니다. [`Color`](../textstyle/color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | 텍스트 스타일의 배경 패턴을 가져오거나 설정합니다. [`BackgroundPattern`](../textstyle/backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | 텍스트의 색을 가져오거나 설정합니다. |
| [Field](../../aspose.tasks.visualization/tabletextstyle/field/) { get; set; } | 스타일이 적용될 필드를 가져오거나 설정합니다. [`Field`](./field/). |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | 텍스트 스타일의 글꼴을 가져오거나 설정합니다. |
| override [ItemType](../../aspose.tasks.visualization/tabletextstyle/itemtype/) { get; } | [`TextItemType`](../textitemtype/) 열거형의 값을 반환합니다. |
| [RowUid](../../aspose.tasks.visualization/tabletextstyle/rowuid/) { get; } | 행 고유 ID를 가져옵니다. 스타일이 보기의 모든 행에 적용되는 경우 -1을 반환합니다. |

## 예제

프로젝트에서 다양한 텍스트 항목을 스타일링하는 데 사용되는 테이블 텍스트 스타일을 사용자 지정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// 첫 번째 작업 이름 텍스트 스타일을 설정합니다
var style1 = new TableTextStyle(1);
// 스타일을 적용할 필드를 설정합니다.
style1.Field = Field.TaskName;
// 텍스트 스타일의 <see cref=\"P:Aspose.Tasks.Visualization.TextStyle.Font\" />을 설정합니다.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// 텍스트 스타일 글꼴의 크기를 포인트 단위로 설정합니다.

// 두 번째 작업 기간 텍스트 스타일을 설정합니다
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // 뷰 데이터를 기록해야 함을 나타내는 플래그를 설정합니다
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### 또 보기

* class [TextStyle](../textstyle/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


