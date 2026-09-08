---
title: "클래스 PageMargins"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.PageMargins 클래스. 인쇄용 페이지 여백을 나타냅니다."
type: docs
weight: 3230
url: /ko/net/aspose.tasks.visualization/pagemargins/
---
## PageMargins class

인쇄용 페이지 여백을 나타냅니다.

```csharp
public class PageMargins
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PageMargins](pagemargins/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Borders](../../aspose.tasks.visualization/pagemargins/borders/) { get; set; } | 테두리를 인쇄할 위치를 가져오거나 설정합니다. [`Border`](../border/) 열거형의 값 중 하나일 수 있습니다. |
| [Bottom](../../aspose.tasks.visualization/pagemargins/bottom/) { get; set; } | 하단 여백의 크기를 센티미터 단위로 가져오거나 설정합니다. |
| [Left](../../aspose.tasks.visualization/pagemargins/left/) { get; set; } | 왼쪽 여백의 크기를 센티미터 단위로 가져오거나 설정합니다. |
| [Right](../../aspose.tasks.visualization/pagemargins/right/) { get; set; } | 오른쪽 여백의 크기를 센티미터 단위로 가져오거나 설정합니다. |
| [Top](../../aspose.tasks.visualization/pagemargins/top/) { get; set; } | 상단 여백의 크기를 센티미터 단위로 가져오거나 설정합니다. |

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


