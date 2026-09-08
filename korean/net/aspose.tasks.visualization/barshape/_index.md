---
title: "열거형 BarShape"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.BarShape 열거형. 막대 사각형의 모양"
type: docs
weight: 2950
url: /ko/net/aspose.tasks.visualization/barshape/
---
## BarShape enumeration

막대 사각형의 모양입니다.

```csharp
public enum BarShape
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Full | `0` | 전체 사각형 막대 모양을 나타냅니다. |
| HalfHeight | `1` | 상단 정렬된 절반 높이 사각형 막대 모양을 나타냅니다. |
| HalfHeightBottom | `2` | 하단 정렬된 절반 높이 사각형 막대 모양을 나타냅니다. |
| Thin | `3` | 중앙 정렬된 선 모양을 나타냅니다. |
| None | `4` | 없음 막대 모양을 나타냅니다. |
| Middle | `5` | 중앙 정렬된 선 모양을 나타냅니다. |
| LineBottom | `6` | 하단 정렬된 선 모양을 나타냅니다. |
| LineTop | `7` | 상단 정렬된 선 모양을 나타냅니다. |

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


