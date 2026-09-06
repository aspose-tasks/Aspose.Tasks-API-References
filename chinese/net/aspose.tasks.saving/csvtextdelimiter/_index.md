---
title: "枚举 CsvTextDelimiter"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.CsvTextDelimiter 枚举。CSV 格式的文本分隔符"
type: docs
weight: 1990
url: /zh/net/aspose.tasks.saving/csvtextdelimiter/
---
## CsvTextDelimiter enumeration

CSV 格式的文本分隔符。

```csharp
public enum CsvTextDelimiter
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Comma | `0` | 逗号分隔符。 |
| Semicolon | `1` | 分号分隔符。 |
| Space | `2` | 空格分隔符。 |
| Tab | `3` | 制表符分隔符。 |

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


