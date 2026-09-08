---
title: "CsvOptions.Encoding"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CsvOptions 속성. CSV를 저장할 인코딩을 가져오거나 설정합니다"
type: docs
weight: 30
url: /ko/net/aspose.tasks.saving/csvoptions/encoding/
---
## CsvOptions.Encoding property

CSV를 저장할 인코딩을 가져오거나 설정합니다.

```csharp
public Encoding Encoding { get; set; }
```

## 예제

CSV 파일로 프로젝트를 저장하는 방법을 보여줍니다 &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; 사용

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

### 또 보기

* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


