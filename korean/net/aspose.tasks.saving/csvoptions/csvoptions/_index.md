---
title: "CsvOptions.CsvOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CsvOptions 생성자. CSV 형식으로 프로젝트를 저장하는 데 사용할 수 있는 CsvOptions 클래스의 새 인스턴스를 초기화합니다"
type: docs
weight: 10
url: /ko/net/aspose.tasks.saving/csvoptions/csvoptions/
---
## CsvOptions constructor

CSV 형식으로 프로젝트를 저장하는 데 사용할 수 있는 [`CsvOptions`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public CsvOptions()
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


