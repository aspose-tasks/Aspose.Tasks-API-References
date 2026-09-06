---
title: "ImageSaveOptions.Pages"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ImageSaveOptions 属性。获取或设置在将项目布局保存为单独文件时要保存的页码列表。如果此列表为空，则会保存所有页。"
type: docs
weight: 50
url: /zh/net/aspose.tasks.saving/imagesaveoptions/pages/
---
## ImageSaveOptions.Pages property

获取或设置在将项目布局保存为单独文件时要保存的页码列表。如果此列表为空，则会保存所有页面。

```csharp
public List<int> Pages { get; set; }
```

## 示例

展示如何将选定的页面保存为图像。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
                  {
                      RenderToSinglePage = false,
                      StartDate = project.Get(Prj.StartDate),
                      EndDate = project.Get(Prj.FinishDate),
                      PageSize = PageSize.Letter
                  };
options.Pages.Add(2);

project.Save(OutDir + "SaveSelectedPagesImageSaveOptions_page2_out.jpeg", options);
```

### 另见

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


