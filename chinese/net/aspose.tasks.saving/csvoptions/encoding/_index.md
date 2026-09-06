---
title: "CsvOptions.Encoding"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CsvOptions 属性。获取或设置用于保存 CSV 的编码"
type: docs
weight: 30
url: /zh/net/aspose.tasks.saving/csvoptions/encoding/
---
## CsvOptions.Encoding property

获取或设置用于保存 CSV 的编码。

```csharp
public Encoding Encoding { get; set; }
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


