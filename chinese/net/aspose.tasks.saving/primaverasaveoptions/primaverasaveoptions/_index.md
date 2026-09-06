---
title: "PrimaveraSaveOptions.PrimaveraSaveOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PrimaveraSaveOptions 构造函数。初始化 PrimaveraSaveOptions 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks.saving/primaverasaveoptions/primaverasaveoptions/
---
## PrimaveraSaveOptions constructor

初始化 [`PrimaveraSaveOptions`](../) 类的新实例。

```csharp
public PrimaveraSaveOptions()
```

## 示例

展示如何使用 &lt;see cref="Aspose.Tasks.Saving.PrimaveraSaveOptions" /&gt;。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// 创建 Primavera 保存选项并进行调优
var options = new PrimaveraSaveOptions
                  {
                      // 定义活动的前缀和后缀
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // 控制活动的重新编号
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### 另见

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


