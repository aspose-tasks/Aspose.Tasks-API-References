---
title: "열거형 DataCategory"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.DataCategory 열거형. CSV로 저장할 때 사용되는 데이터 범주입니다."
type: docs
weight: 2000
url: /ko/net/aspose.tasks.saving/datacategory/
---
## DataCategory enumeration

CSV로 저장할 때 사용되는 데이터 범주입니다.

```csharp
public enum DataCategory
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Tasks | `0` | 작업 정보. |
| Resources | `1` | 리소스 정보. |
| Assignments | `2` | 할당 정보. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


