---
title: "열거형 CsvTextDelimiter"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.CsvTextDelimiter 열거형. CSV 형식의 텍스트 구분자."
type: docs
weight: 1990
url: /ko/net/aspose.tasks.saving/csvtextdelimiter/
---
## CsvTextDelimiter enumeration

CSV 형식의 텍스트 구분자입니다.

```csharp
public enum CsvTextDelimiter
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Comma | `0` | 쉼표 구분자. |
| Semicolon | `1` | 세미콜론 구분자. |
| Space | `2` | 공백 구분자. |
| Tab | `3` | 탭 구분자. |

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


