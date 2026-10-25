---
title: "枚举 DataCategory"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.DataCategory 枚举。保存为 CSV 时使用的数据类别"
type: docs
weight: 2000
url: /zh/net/aspose.tasks.saving/datacategory/
---
## DataCategory enumeration

保存为 CSV 时使用的数据类别。

```csharp
public enum DataCategory
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Tasks | `0` | 任务信息。 |
| Resources | `1` | 资源信息。 |
| Assignments | `2` | 分配信息。 |

## 示例

展示如何使用 &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; 将项目保存为 CSV 文件。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var options = new CsvOptions
{
    DataCategory = DataCategory.Resources,
    TextDelimiter = CsvTextDelimiter.Semicolon,
    Encoding = Encoding.Unicode, IncludeHeaders = true
};

project.Save(OutDir + "WorkWithCsvOptions_out.csv", options);
```

### 另见

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


