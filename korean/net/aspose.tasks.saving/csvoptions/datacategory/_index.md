---
title: "CsvOptions.DataCategory"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CsvOptions 속성. 저장될 데이터 카테고리를 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.saving/csvoptions/datacategory/
---
## CsvOptions.DataCategory property

저장될 데이터 범주를 가져오거나 설정합니다.

```csharp
public DataCategory DataCategory { get; set; }
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

* enum [DataCategory](../../datacategory/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


