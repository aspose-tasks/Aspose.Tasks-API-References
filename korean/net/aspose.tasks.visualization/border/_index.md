---
title: "Enum Border"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.Border 열거형. 테두리 유형을 지정합니다."
type: docs
weight: 2970
url: /ko/net/aspose.tasks.visualization/border/
---
## Border enumeration

테두리 유형을 지정합니다.

```csharp
public enum Border
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| NoBorder | `0` | 테두리 없음. |
| AroundEveryPage | `1` | 모든 페이지 주변. |
| OutsidePages | `2` | 외부 페이지에서. |

## 예제

페이지 여백을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 기본 보기를 수정합니다.
var margins = project.DefaultView.PageInfo.Margins;

// 여백을 수정합니다.
margins.Left = 10d;
margins.Top = 10d;
margins.Right = 10d;
margins.Bottom = 10d;
margins.Borders = Border.OutsidePages;

project.Save(OutDir + "WorkWithPageMargins_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


