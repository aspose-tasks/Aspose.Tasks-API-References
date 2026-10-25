---
title: "SaveOptions.TextStyles"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SaveOptions 属性。获取或设置在项目视图渲染期间应用的文本样式列表"
type: docs
weight: 190
url: /zh/net/aspose.tasks.saving/saveoptions/textstyles/
---
## SaveOptions.TextStyles property

获取或设置在项目视图渲染期间应用的文本样式列表。

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## 备注

这些样式会覆盖在 GanttCharView.TextStyles 中定义的样式。

## 示例

展示如何使用保存选项的文本样式，这些样式用于为项目中的不同文本项设置样式。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Bold | FontStyles.Italic)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};

project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### 另见

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


