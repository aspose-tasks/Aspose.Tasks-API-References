---
title: "CsvOptions.IncludeHeaders"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CsvOptions 속성. 헤더를 포함할지 여부를 나타내는 값을 가져오거나 설정합니다. 기본값은 TRUE입니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks.saving/csvoptions/includeheaders/
---
## CsvOptions.IncludeHeaders property

헤더를 포함할지 여부를 나타내는 값을 가져오거나 설정합니다(기본값은 TRUE).

```csharp
public bool IncludeHeaders { get; set; }
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


