---
title: "枚举 BackgroundPattern"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.BackgroundPattern 枚举。指定背景图案"
type: docs
weight: 100
url: /zh/net/aspose.tasks/backgroundpattern/
---
## BackgroundPattern enumeration

指定背景图案。

```csharp
public enum BackgroundPattern
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| DarkDiagonalLeft | `7` | 表示暗左对角线背景图案。 |
| DarkDiagonalRight | `8` | 表示暗右对角线背景图案。 |
| DarkDither | `13` | 表示暗抖动背景图案。 |
| DarkFill | `4` | 表示暗填充背景图案。 |
| DiagonalLeft | `5` | 指示左对角线背景图案。 |
| DiagonalRight | `6` | 指示右对角线背景图案。 |
| Hollow | `0` | 指示空心背景图案。 |
| LightDither | `11` | 指示浅色抖动背景图案。 |
| LightFill | `2` | 指示浅色填充背景图案。 |
| MediumDither | `12` | 指示中等抖动背景图案。 |
| MediumFill | `3` | 指示中等填充背景图案。 |
| MediumVerticalStripe | `10` | 指示中等垂直条纹背景图案。 |
| SolidFill | `1` | 指示实心填充背景图案。 |
| ThinVerticalStripe | `9` | 指示细垂直条纹背景图案。 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


