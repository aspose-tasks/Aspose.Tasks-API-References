---
title: "열거형 Shape"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.Shape 열거형. 막대 스타일의 시작 또는 끝에 표시되는 마커 형태이며, 일부 SaveFileFormat에 뷰 데이터를 저장할 때 렌더링됩니다."
type: docs
weight: 3360
url: /ko/net/aspose.tasks.visualization/shape/
---
## Shape enumeration

일부 [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/)에 뷰 데이터를 저장할 때 렌더링되는 막대 스타일의 시작 또는 끝에 있는 마커의 형태.

```csharp
public enum Shape
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| None | `0` | None 형태를 나타냅니다. |
| VerticalLine | `1` | 수직 선 형태를 나타냅니다. |
| Pentagon | `2` | 오각형 형태를 나타냅니다. |
| Triangle | `3` | 삼각형 형태를 나타냅니다. |
| LeftBracket | `4` | 왼쪽 대괄호 형태를 나타냅니다. |
| RightBracket | `5` | 오른쪽 대괄호 형태를 나타냅니다. |
| ArrowDown | `6` | 아래쪽 화살표 형태를 나타냅니다. |
| LeftFade | `7` | 왼쪽 페이드 형태를 나타냅니다. |
| RightFade | `8` | 오른쪽 페이드 형태를 나타냅니다. |
| Diamond | `9` | 다이아몬드 형태를 나타냅니다. |
| Circle | `10` | 원형 형태를 나타냅니다. |

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


