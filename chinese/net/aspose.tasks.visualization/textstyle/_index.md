---
title: "类 TextStyle"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.TextStyle 类。更改项目视图中项目的文本的视觉样式"
type: docs
weight: 3420
url: /zh/net/aspose.tasks.visualization/textstyle/
---
## TextStyle class

更改项目视图中项目文本的视觉样式。

```csharp
public class TextStyle
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [TextStyle](textstyle/#constructor)() | 使用默认设置初始化 `TextStyle` 类的新实例。 |
| [TextStyle](textstyle/#constructor_1)(FontDescriptor) | 使用指定的字体设置初始化 `TextStyle` 类的新实例。 |
| [TextStyle](textstyle/#constructor_2)(FontStyles) | 使用默认字体和指定的字体样式初始化 `TextStyle` 类的新实例。 |
| [TextStyle](textstyle/#constructor_3)(float, FontStyles) | 使用默认字体以及指定的字体大小和样式初始化 `TextStyle` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | 获取或设置文本样式的背景颜色。[`Color`](./color/)。 |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | 获取或设置文本样式的背景图案。[`BackgroundPattern`](./backgroundpattern/)。 |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | 获取或设置文本的颜色。 |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | 获取或设置文本样式的字体。 |
| virtual [ItemType](../../aspose.tasks.visualization/textstyle/itemtype/) { get; set; } | 获取或设置文本样式的 [`TextItemType`](../textitemtype/)。 |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


