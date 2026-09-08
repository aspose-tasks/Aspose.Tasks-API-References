---
title: "열거형 CostAccrualType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.CostAccrualType 열거형. 발생 비용의 유형을 지정합니다."
type: docs
weight: 350
url: /ko/net/aspose.tasks/costaccrualtype/
---
## CostAccrualType enumeration

발생 비용 유형을 지정합니다.

```csharp
public enum CostAccrualType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `-1` | 정의되지 않은 값은 해당 필드가 원본 프로젝트 파일에 정의되지 않았음을 나타냅니다. |
| Start | `0` | Start 비용 발생 유형을 나타냅니다. |
| Prorated | `1` | Prorated 비용 발생 유형을 나타냅니다. |
| End | `2` | End 비용 발생 유형을 나타냅니다. |
| Invalid | `3` | Invalid 비용 발생 유형을 나타냅니다. |

## 비고

XML로 내보내는 동안 Undefined 값은 결과 XML에서 제거됩니다.

## 예제

리소스 표준 및 초과 근무 비용이 언제 청구되거나 발생되는지(발생 방법: 리소스 비용이 발생하는 시점과 실제 비용이 프로젝트에 청구되는 시점을 결정합니다. 작업의 시작 [Start] 또는 종료 [End] 시점에 비용을 발생시키거나 작업 중에 [Prorated]로 비례 배분할 수 있습니다.)를 작업 비용에 적용하는 방법을 보여줍니다 (CostAccrualType.End).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);
// 비용 발생 유형 설정
// End 옵션을 선택하면 남은 작업이 0이 될 때까지 비용이 발생하지 않습니다.
resource.Set(Rsc.AccrueAt, CostAccrualType.End);
// 프로젝트와 작업...
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


