---
title: "CsvOptions.CsvOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CsvOptions 构造函数。初始化 CsvOptions 类的新实例，可用于以 CSV 格式保存项目"
type: docs
weight: 10
url: /zh/net/aspose.tasks.saving/csvoptions/csvoptions/
---
## CsvOptions constructor

初始化 [`CsvOptions`](../) 类的新实例，可用于以 CSV 格式保存项目。

```csharp
public CsvOptions()
```

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

* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


