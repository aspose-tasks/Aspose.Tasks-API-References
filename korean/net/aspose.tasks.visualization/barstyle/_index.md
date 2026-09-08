---
title: "클래스 BarStyle"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.BarStyle 클래스. 프로젝트 보기에서 항목의 막대 시각적 스타일을 변경합니다."
type: docs
weight: 2960
url: /ko/net/aspose.tasks.visualization/barstyle/
---
## BarStyle class

프로젝트 보기에서 항목의 막대 시각 스타일을 변경합니다.

```csharp
public class BarStyle
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [BarStyle](barstyle/)() | `BarStyle` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [BarColor](../../aspose.tasks.visualization/barstyle/barcolor/) { get; set; } | 막대 스타일의 색상을 가져오거나 설정합니다. |
| [BarShape](../../aspose.tasks.visualization/barstyle/barshape/) { get; set; } | 막대 스타일의 [`BarShape`](./barshape/)을 가져오거나 설정합니다. |
| [BottomBarTextConverter](../../aspose.tasks.visualization/barstyle/bottombartextconverter/) { get; set; } | 작업 막대의 하단에 표시할 텍스트를 가져오기 위한 사용자 정의 변환기를 가져오거나 설정합니다. [`BottomField`](./bottomfield/) 속성의 값을 재정의합니다. |
| [BottomField](../../aspose.tasks.visualization/barstyle/bottomfield/) { get; set; } | 막대 하단에 표시될 필드를 가져오거나 설정합니다. |
| [EndShape](../../aspose.tasks.visualization/barstyle/endshape/) { get; set; } | 막대 끝의 [`Shape`](../shape/)을 가져오거나 설정합니다. |
| [EndShapeColor](../../aspose.tasks.visualization/barstyle/endshapecolor/) { get; set; } | 막대 끝에 있는 모양의 색상을 가져오거나 설정합니다. |
| [EndShapeType](../../aspose.tasks.visualization/barstyle/endshapetype/) { get; set; } | 끝 모양의 유형을 가져오거나 설정합니다. [`GanttBarType`](../ganttbartype/). |
| [From](../../aspose.tasks.visualization/barstyle/from/) { get; set; } | 간트 막대의 시작 지점 위치를 가져오거나 설정합니다. [`Field`](../../aspose.tasks/field/). |
| [InsideBarTextConverter](../../aspose.tasks.visualization/barstyle/insidebartextconverter/) { get; set; } | 작업 막대 내부에 표시할 텍스트를 가져오기 위한 사용자 정의 변환기를 가져오거나 설정합니다. [`InsideField`](./insidefield/) 속성의 값을 재정의합니다. |
| [InsideField](../../aspose.tasks.visualization/barstyle/insidefield/) { get; set; } | 막대 내부에 표시될 필드를 가져오거나 설정합니다. |
| [ItemType](../../aspose.tasks.visualization/barstyle/itemtype/) { get; set; } | 막대 스타일의 [`BarItemType`](../baritemtype/)을 가져오거나 설정합니다. |
| [LeftBarTextConverter](../../aspose.tasks.visualization/barstyle/leftbartextconverter/) { get; set; } | 작업 막대 왼쪽에 렌더링할 텍스트를 가져오기 위한 사용자 정의 변환기를 가져오거나 설정합니다. [`LeftField`](./leftfield/) 속성 값을 재정의합니다. |
| [LeftField](../../aspose.tasks.visualization/barstyle/leftfield/) { get; set; } | 막대 왼쪽에 표시될 필드를 가져오거나 설정합니다. |
| [RightBarTextConverter](../../aspose.tasks.visualization/barstyle/rightbartextconverter/) { get; set; } | 작업 막대 오른쪽에 표시할 텍스트를 가져오기 위한 사용자 정의 변환기를 가져오거나 설정합니다. [`RightField`](./rightfield/) 속성의 값을 재정의합니다. |
| [RightField](../../aspose.tasks.visualization/barstyle/rightfield/) { get; set; } | 막대 오른쪽에 표시될 필드를 가져오거나 설정합니다. |
| [StartShape](../../aspose.tasks.visualization/barstyle/startshape/) { get; set; } | 막대 시작 부분의 [`Shape`](../shape/)을 가져오거나 설정합니다. |
| [StartShapeColor](../../aspose.tasks.visualization/barstyle/startshapecolor/) { get; set; } | 막대 시작 부분의 도형 색상을 가져오거나 설정합니다. |
| [StartShapeType](../../aspose.tasks.visualization/barstyle/startshapetype/) { get; set; } | 시작 모양의 유형을 가져오거나 설정합니다. |
| [TextStyle](../../aspose.tasks.visualization/barstyle/textstyle/) { get; set; } | 막대 텍스트의 스타일을 가져오거나 설정합니다. |
| [To](../../aspose.tasks.visualization/barstyle/to/) { get; set; } | 간트 막대의 종료 지점 위치를 가져오거나 설정합니다. |
| [TopBarTextConverter](../../aspose.tasks.visualization/barstyle/topbartextconverter/) { get; set; } | 작업 막대의 상단에 표시할 텍스트를 가져오기 위한 사용자 정의 변환기를 가져오거나 설정합니다. [`TopField`](./topfield/) 속성의 값을 재정의합니다. |
| [TopField](../../aspose.tasks.visualization/barstyle/topfield/) { get; set; } | 막대 상단에 표시될 필드를 가져오거나 설정합니다. |

## 예제

사용자 정의 막대 스타일을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    BarStyles = new List<BarStyle>()
};

// 마일스톤 작업에 대한 막대 스타일을 추가합니다.
var style = new BarStyle();
// 막대 스타일의 <see cref=\"T:Aspose.Tasks.Visualization.BarItemType\" />를 설정합니다.
style.ItemType = BarItemType.Milestone;
// 막대 스타일의 <see cref=\"T:System.Drawing.Color\" />를 설정합니다.
style.BarColor = Color.Green;
// 막대 스타일의 <see cref=\"P:Aspose.Tasks.Visualization.BarStyle.BarShape\" />를 설정합니다.
style.BarShape = BarShape.HalfHeight;
// 막대 시작 부분에 <see cref="T:Aspose.Tasks.Visualization.Shape" />를 설정합니다
style.StartShape = Shape.LeftBracket;
// 막대 시작 부분에 도형의 <see cref="T:System.Drawing.Color" />를 설정합니다
style.StartShapeColor = Color.Aqua;
// 막대 끝 부분에 <see cref="T:Aspose.Tasks.Visualization.Shape" />를 설정합니다
style.EndShape = Shape.RightBracket;
// 막대 끝 부분에 도형의 <see cref="T:System.Drawing.Color" />를 설정합니다
style.EndShapeColor = Color.Aquamarine;
// 막대 오른쪽에 표시할 텍스트를 설정합니다.
style.TextStyle = new TextStyle();
style.TextStyle.BackgroundColor = Color.Black;

// 막대의 텍스트를 변환할 수 있는 기능이 존재합니다.
// 막대에 표시할 텍스트를 가져오기 위해 변환기를 설정합니다.
style.LeftBarTextConverter = task =>
{
    if (!task.Get(Tsk.Name).StartsWith("T"))
    {
        task.Set(Tsk.Name, "T" + task.Get(Tsk.Name));
    }

    return task.Get(Tsk.Name);
};

options.BarStyles.Add(style);

// 프로젝트를 저장합니다
project.Save(OutDir + "WorkWithBarStyle_out.mpp", options);
```

### 또 보기

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


