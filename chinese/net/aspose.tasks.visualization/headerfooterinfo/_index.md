---
title: "类 HeaderFooterInfo"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.HeaderFooterInfo 类。表示用于打印和视图渲染的页眉页脚或图例的可视内容。"
type: docs
weight: 3130
url: /zh/net/aspose.tasks.visualization/headerfooterinfo/
---
## HeaderFooterInfo class

表示用于视图的打印\渲染的页眉、页脚或图例的视觉内容。

```csharp
public class HeaderFooterInfo
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [HeaderFooterInfo](headerfooterinfo/)() | 初始化 `HeaderFooterInfo` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | 获取或设置在父元素中显示的居中图像。 |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | 获取或设置居中图像的显示尺寸。 |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | 获取或设置在父元素中显示的居中文本。 |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | 获取或设置在父元素中显示的左对齐图像。 |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | 获取或设置左图像的显示尺寸。 |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | 获取或设置在父元素中显示的左对齐文本。 |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | 获取或设置在父元素中显示的右对齐图像。 |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | 获取或设置右图像的显示尺寸。 |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | 获取或设置在父元素中显示的右对齐文本。 |

## 示例

显示如何读取页面页眉/页脚信息。

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

### 另见

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


