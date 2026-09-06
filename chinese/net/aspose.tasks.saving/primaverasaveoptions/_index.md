---
title: "类 PrimaveraSaveOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.PrimaveraSaveOptions 类。允许在将项目保存为 Primavera XER 格式时指定其他选项"
type: docs
weight: 2150
url: /zh/net/aspose.tasks.saving/primaverasaveoptions/
---
## PrimaveraSaveOptions class

允许在将项目保存为 Primavera XER 格式时指定附加选项。

```csharp
public class PrimaveraSaveOptions : SimpleSaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PrimaveraSaveOptions](primaverasaveoptions/)() | 初始化 `PrimaveraSaveOptions` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [ActivityIdIncrement](../../aspose.tasks.saving/primaverasaveoptions/activityidincrement/) { get; set; } | 获取或设置在活动 ID 重编号中使用的增量。 |
| [ActivityIdPrefix](../../aspose.tasks.saving/primaverasaveoptions/activityidprefix/) { get; set; } | 获取或设置在活动 ID 重编号中使用的前缀。 |
| [ActivityIdSuffix](../../aspose.tasks.saving/primaverasaveoptions/activityidsuffix/) { get; set; } | 获取或设置在活动 ID 重编号中使用的后缀。 |
| [RenumberActivityIds](../../aspose.tasks.saving/primaverasaveoptions/renumberactivityids/) { get; set; } | 获取或设置一个值，指示是否需要重新编号活动 ID。 |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 获取或设置如果使用此保存选项对象，文档将被保存的格式。 |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/) { get; set; } | 获取或设置一个值，指示在导出期间是否应跳过资源对汇总任务的分配。 |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 获取或设置用于在甘特图和任务表图上排序任务的比较器。 |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 获取或设置用于过滤在甘特图、任务表和任务使用图上渲染的任务的条件。 |

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


