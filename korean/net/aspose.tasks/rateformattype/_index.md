---
title: "열거형 RateFormatType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.RateFormatType 열거형. Microsoft Project에서 요금을 표시하는 데 사용되는 단위를 지정합니다."
type: docs
weight: 1640
url: /ko/net/aspose.tasks/rateformattype/
---
## RateFormatType enumeration

Microsoft Project에서 비율을 표시하는 데 사용되는 단위를 지정합니다.

```csharp
public enum RateFormatType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `-1` | 값이 원본 프로젝트 파일에 정의되지 않았습니다. |
| Minute | `0` | 분 ("min") |
| Hour | `1` | 시간 ("hr") |
| Day | `2` | 일 ("day") |
| Week | `3` | 주 ("wk") |
| Month | `4` | 월 ("mo") |
| Year | `5` | 년 ("yr") |
| MaterialResourceRate | `6` | 재료 리소스 요금 (비어 있음) |

## 비고

XML로 내보내는 동안 Undefined 값은 결과 XML에서 제거됩니다.

## 예제

Rsc.StandardRateFormat 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


