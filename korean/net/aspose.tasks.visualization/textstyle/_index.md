---
title: "클래스 TextStyle"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.TextStyle 클래스. 프로젝트 보기에서 항목의 텍스트 시각적 스타일을 변경합니다"
type: docs
weight: 3420
url: /ko/net/aspose.tasks.visualization/textstyle/
---
## TextStyle class

프로젝트 보기에서 항목의 텍스트 시각 스타일을 변경합니다.

```csharp
public class TextStyle
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [TextStyle](textstyle/#constructor)() | `TextStyle` 클래스의 새 인스턴스를 기본 설정으로 초기화합니다. |
| [TextStyle](textstyle/#constructor_1)(FontDescriptor) | 지정된 글꼴 설정으로 `TextStyle` 클래스의 새 인스턴스를 초기화합니다. |
| [TextStyle](textstyle/#constructor_2)(FontStyles) | 기본 글꼴과 지정된 글꼴 스타일을 사용하여 `TextStyle` 클래스의 새 인스턴스를 초기화합니다. |
| [TextStyle](textstyle/#constructor_3)(float, FontStyles) | 기본 글꼴과 지정된 글꼴 크기 및 스타일을 사용하여 `TextStyle` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | 텍스트 스타일의 배경 색을 가져오거나 설정합니다. [`Color`](./color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | 텍스트 스타일의 배경 패턴을 가져오거나 설정합니다. [`BackgroundPattern`](./backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | 텍스트의 색을 가져오거나 설정합니다. |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | 텍스트 스타일의 글꼴을 가져오거나 설정합니다. |
| virtual [ItemType](../../aspose.tasks.visualization/textstyle/itemtype/) { get; set; } | 텍스트 스타일의 [`TextItemType`](../textitemtype/)을 가져오거나 설정합니다. |

## 예제

프로젝트에서 다양한 텍스트 항목을 스타일링하는 데 사용되는 텍스트 스타일을 사용자 정의하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle();
style.Color = Color.OrangeRed;
style.Font = new FontDescriptor(FontFamily.GenericMonospace.Name, 10F, FontStyles.Bold | FontStyles.Italic);
style.ItemType = TextItemType.OverallocatedResources;
style.BackgroundColor = Color.Aqua;
style.BackgroundPattern = BackgroundPattern.DarkDither;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### 또 보기

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


