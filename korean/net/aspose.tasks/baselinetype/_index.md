---
title: "열거형 BaselineType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.BaselineType 열거형. 분산 값을 계산하는 데 사용되는 기준선 유형을 지정합니다."
type: docs
weight: 130
url: /ko/net/aspose.tasks/baselinetype/
---
## BaselineType enumeration

분산 값을 계산하는 데 사용되는 기준선 유형을 지정합니다.

```csharp
public enum BaselineType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `-1` | 원본 프로젝트 파일에 해당 필드가 정의되지 않았음을 나타냅니다. |
| Baseline | `0` | Baseline 유형을 나타냅니다. |
| Baseline1 | `1` | Baseline1 유형을 나타냅니다. |
| Baseline2 | `2` | Baseline2 유형을 나타냅니다. |
| Baseline3 | `3` | Baseline3 유형을 나타냅니다. |
| Baseline4 | `4` | Baseline4 유형을 나타냅니다. |
| Baseline5 | `5` | Baseline5 유형을 나타냅니다. |
| Baseline6 | `6` | Baseline6 유형을 나타냅니다. |
| Baseline7 | `7` | Baseline7 유형을 나타냅니다. |
| Baseline8 | `8` | Baseline8 유형을 나타냅니다. |
| Baseline9 | `9` | Baseline9 유형을 나타냅니다. |
| Baseline10 | `10` | Baseline10 유형을 나타냅니다. |

## 비고

XML로 내보내는 동안 Undefined 값은 결과 XML에서 제거됩니다.

## 예제

프로젝트에 대한 기준선을 설정하는 방법을 보여줍니다 (BaselineType.Baseline).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// 전체 프로젝트에 대해 지정된 기준선에 기준선 필드를 저장합니다.
project.SetBaseline(BaselineType.Baseline);
// 프로젝트의 기준선 작업...
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


