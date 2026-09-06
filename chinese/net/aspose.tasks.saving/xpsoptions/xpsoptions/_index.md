---
title: "XpsOptions.XpsOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "XpsOptions 构造函数。初始化 XpsOptions 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks.saving/xpsoptions/xpsoptions/
---
## XpsOptions constructor

初始化 [`XpsOptions`](../) 类的新实例。

```csharp
public XpsOptions()
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


