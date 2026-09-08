---
title: "CsvOptions.TextDelimiter"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CsvOptions 속성. 텍스트 구분자를 가져오거나 설정합니다"
type: docs
weight: 50
url: /ko/net/aspose.tasks.saving/csvoptions/textdelimiter/
---
## CsvOptions.TextDelimiter property

텍스트 구분자를 가져오거나 설정합니다.

```csharp
public CsvTextDelimiter TextDelimiter { get; set; }
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

* enum [CsvTextDelimiter](../../csvtextdelimiter/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


