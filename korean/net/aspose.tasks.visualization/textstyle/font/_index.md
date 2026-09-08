---
title: "TextStyle.Font"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TextStyle 속성. 텍스트 스타일의 글꼴을 가져오거나 설정합니다"
type: docs
weight: 50
url: /ko/net/aspose.tasks.visualization/textstyle/font/
---
## TextStyle.Font property

텍스트 스타일의 글꼴을 가져오거나 설정합니다.

```csharp
public FontDescriptor Font { get; set; }
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

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


