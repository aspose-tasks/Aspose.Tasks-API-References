---
title: "TextStyle.BackgroundColor"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TextStyle 속성. 텍스트 스타일의 배경 색상을 가져오거나 설정합니다. Color"
type: docs
weight: 20
url: /ko/net/aspose.tasks.visualization/textstyle/backgroundcolor/
---
## TextStyle.BackgroundColor property

텍스트 스타일의 배경 색상을 가져오거나 설정합니다. [`Color`](../color/).

```csharp
public Color BackgroundColor { get; set; }
```

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

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


