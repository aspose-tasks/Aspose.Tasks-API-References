---
title: "CsvOptions.DataCategory"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CsvOptions 属性。获取或设置要保存的数据类别"
type: docs
weight: 20
url: /zh/net/aspose.tasks.saving/csvoptions/datacategory/
---
## CsvOptions.DataCategory property

获取或设置要保存的数据类别。

```csharp
public DataCategory DataCategory { get; set; }
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

* enum [DataCategory](../../datacategory/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


