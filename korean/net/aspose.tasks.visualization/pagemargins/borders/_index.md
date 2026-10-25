---
title: "PageMargins.Borders"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PageMargins 속성. 테두리를 인쇄할 위치를 가져오거나 설정합니다. Border 열거형의 값 중 하나일 수 있습니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.visualization/pagemargins/borders/
---
## PageMargins.Borders property

테두리를 인쇄할 위치를 가져오거나 설정합니다. [`Border`](../../border/) 열거형의 값 중 하나일 수 있습니다.

```csharp
public Border Borders { get; set; }
```

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

* enum [Border](../../border/)
* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


