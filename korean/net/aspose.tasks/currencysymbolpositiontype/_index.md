---
title: "열거형 CurrencySymbolPositionType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.CurrencySymbolPositionType 열거형. 통화 기호의 위치를 지정합니다."
type: docs
weight: 370
url: /ko/net/aspose.tasks/currencysymbolpositiontype/
---
## CurrencySymbolPositionType enumeration

통화 기호의 위치를 지정합니다.

```csharp
public enum CurrencySymbolPositionType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `-1` | 정의되지 않은 값은 해당 필드가 원본 프로젝트 파일에 정의되지 않았음을 나타냅니다. |
| Before | `0` | 통화 기호 앞 위치 유형을 나타냅니다. |
| After | `1` | 통화 기호 뒤 위치 유형을 나타냅니다. |
| BeforeWithSpace | `2` | 통화 기호 앞에 공백이 있는 위치 유형을 나타냅니다. |
| AfterWithSpace | `3` | 통화 기호 뒤에 공백이 있는 위치 유형을 나타냅니다. |

## 비고

XML로 내보내는 동안 Undefined 값은 결과 XML에서 제거됩니다.

## 예제

통화 기호의 배치를 지정하는 방법을 보여줍니다 (CurrencySymbolPositionType.Before).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// 통화 기호의 배치를 설정합니다
// 앞, 공백 없음 ($0).
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.Before);
// 프로젝트와 작업...
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


