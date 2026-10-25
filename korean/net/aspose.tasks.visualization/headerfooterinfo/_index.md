---
title: "클래스 HeaderFooterInfo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.HeaderFooterInfo 클래스. 뷰의 인쇄 및 렌더링에 사용되는 머리글/바닥글 또는 범례의 시각적 콘텐츠를 나타냅니다."
type: docs
weight: 3130
url: /ko/net/aspose.tasks.visualization/headerfooterinfo/
---
## HeaderFooterInfo class

보기의 인쇄 \ 렌더링에 사용되는 머리글, 바닥글 또는 범례의 시각적 내용을 나타냅니다.

```csharp
public class HeaderFooterInfo
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [HeaderFooterInfo](headerfooterinfo/)() | `HeaderFooterInfo` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | 부모 요소에 표시될 중앙 이미지를 가져오거나 설정합니다. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | 중앙 이미지의 표시 크기를 가져오거나 설정합니다. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | 부모 요소에 표시될 중앙 텍스트를 가져오거나 설정합니다. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | 부모 요소에 표시될 왼쪽 정렬된 이미지를 가져오거나 설정합니다. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | 왼쪽 이미지의 표시 크기를 가져오거나 설정합니다. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | 부모 요소에 표시될 왼쪽 정렬된 텍스트를 가져오거나 설정합니다. |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | 부모 요소에 표시될 오른쪽 정렬된 이미지를 가져오거나 설정합니다. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | 오른쪽 이미지의 표시 크기를 가져오거나 설정합니다. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | 부모 요소에 표시될 오른쪽 정렬된 텍스트를 가져오거나 설정합니다. |

## 예제

페이지 머리글/바닥글 정보를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var info = project.DefaultView.PageInfo;

Console.WriteLine("Header left text: {0} ", info.Header.LeftText);
Console.WriteLine("Header left image: {0} ", info.Header.LeftImage);
Console.WriteLine("Header left image size: {0} ", info.Header.LeftImageSize);
Console.WriteLine("Header center text: {0} ", info.Header.CenteredText);
Console.WriteLine("Header center image: {0} ", info.Header.CenteredImage);
Console.WriteLine("Header center image size: {0} ", info.Header.CenteredImageSize);
Console.WriteLine("Header right text: {0} ", info.Header.RightText);
Console.WriteLine("Header right image: {0} ", info.Header.RightImage);
Console.WriteLine("Header right image size: {0} ", info.Header.RightImageSize);
Console.WriteLine();
Console.WriteLine("Footer left text: {0} ", info.Footer.LeftText);
Console.WriteLine("Footer left image: {0} ", info.Footer.LeftImage);
Console.WriteLine("Footer left image size: {0} ", info.Footer.LeftImageSize);
Console.WriteLine("Footer center text: {0} ", info.Footer.CenteredText);
Console.WriteLine("Footer center image: {0} ", info.Footer.CenteredImage);
Console.WriteLine("Footer center size: {0} ", info.Footer.CenteredImageSize);
Console.WriteLine("Footer right text: {0} ", info.Footer.RightText);
Console.WriteLine("Footer right image: {0} ", info.Footer.RightImage);
Console.WriteLine("Footer right image size: {0} ", info.Footer.RightImageSize);
```

### 또 보기

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


