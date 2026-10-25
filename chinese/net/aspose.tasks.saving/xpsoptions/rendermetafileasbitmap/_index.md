---
title: "XpsOptions.RenderMetafileAsBitmap"
second_title: "Aspose.Tasks for .NET API 参考"
description: "XpsOptions 属性。获取或设置一个值，指示是否应将元文件渲染为位图。"
type: docs
weight: 20
url: /zh/net/aspose.tasks.saving/xpsoptions/rendermetafileasbitmap/
---
## XpsOptions.RenderMetafileAsBitmap property

获取或设置一个值，指示是否将元文件渲染为位图。

```csharp
public bool RenderMetafileAsBitmap { get; set; }
```

## 示例

展示如何将项目保存为 XPS 文件。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// 创建 XPS 保存选项并调整参数
var options = new XpsOptions
{
    RenderMetafileAsBitmap = true
};

project.Save(OutDir + "UseSvgOptions_out.xps", options);
```

### 另见

* class [XpsOptions](../)
* namespace [Aspose.Tasks.Saving](../../xpsoptions/)
* assembly [Aspose.Tasks](../../../)


