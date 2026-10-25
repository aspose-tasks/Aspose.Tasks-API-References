---
title: "FontSettings.SetFontFolders"
second_title: "Aspose.Tasks for .NET API 参考"
description: "FontSettings 方法。设置 Aspose.Tasks 在渲染项目视图时查找 TrueType 字体的文件夹"
type: docs
weight: 50
url: /zh/net/aspose.tasks/fontsettings/setfontfolders/
---
## FontSettings.SetFontFolders method

设置 Aspose.Tasks 在渲染项目视图时查找 TrueType 字体的文件夹。

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontFolders | String[] | 包含 TrueType 字体的文件夹数组。 |
| recursive | Boolean | 如果为 true，指定的文件夹将被递归扫描。 |

## 示例

展示如何设置自定义字体文件夹。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

// 打开的项目中使用的所有字体的 TrueType 字体文件应位于 MyFonts 文件夹中。
options.FontSettings.SetFontFolders(new string[] { "c:\\MyFonts"}, true);

project.Save(OutDir + "EstimatedMilestoneTasks_out4.pdf", options);
```

### 另见

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


