---
title: "열거형 EarnedValueMethodType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.EarnedValueMethodType 열거형. 획득 가치 계산에 사용되는 방법을 지정합니다"
type: docs
weight: 480
url: /ko/net/aspose.tasks/earnedvaluemethodtype/
---
## EarnedValueMethodType enumeration

획득 가치 계산에 사용되는 방법을 지정합니다.

```csharp
public enum EarnedValueMethodType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `-1` | 원본 프로젝트 파일에 필드가 정의되지 않았습니다. |
| PercentComplete | `0` | 완료 비율 |
| PhysicalPercentComplete | `1` | 물리적 완료 비율 |

## 비고

XML로 내보내는 동안 Undefined 값은 결과 XML에서 제거됩니다.

## 예제

획득 가치 계산에 사용되는 방법을 지정하는 방법을 보여줍니다 (EarnedValueMethodType.PercentComplete).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// earned value method type을 'PercentComplete' 로 설정합니다
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
// 프로젝트와 작업...
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


