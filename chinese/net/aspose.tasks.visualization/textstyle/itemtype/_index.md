---
title: "TextStyle.ItemType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TextStyle 属性。获取或设置文本样式的 TextItemType"
type: docs
weight: 60
url: /zh/net/aspose.tasks.visualization/textstyle/itemtype/
---
## TextStyle.ItemType property

获取或设置文本样式的 [`TextItemType`](../../textitemtype/)。

```csharp
public virtual TextItemType ItemType { get; set; }
```

## 示例

展示如何自定义文本样式，这些样式用于为项目中的不同文本项设置样式。

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

### 另见

* enum [TextItemType](../../textitemtype/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


