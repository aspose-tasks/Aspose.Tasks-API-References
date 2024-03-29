---
title: CreateCostTimephased
second_title: .NET API 참조용 Aspose.Tasks
description: 의 새 인스턴스를 만들고 초기화합니다.TimephasedDataaspose.tasks/timephaseddata/ 비용 기반 시간 단계별 데이터 클래스.
type: docs
weight: 20
url: /ko/net/aspose.tasks/timephaseddata/createcosttimephased/
---
## TimephasedData.CreateCostTimephased method

의 새 인스턴스를 만들고 초기화합니다.[`TimephasedData`](../) 비용 기반 시간 단계별 데이터 클래스.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimeUnitType timeUnit, TimephasedDataType type)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| uid | Int32 | 작업의 UID입니다. |
| start | DateTime | 시작 날짜-시간. |
| finish | DateTime | 날짜-시간을 마칩니다. |
| value | Double | 비용 가치. |
| timeUnit | TimeUnitType | 시간 단위 유형. |
| type | TimephasedDataType | 시간대별 데이터 유형. |

### 반환 값

의 인스턴스[`TimephasedData`](../) 비용 기반 시간 단계별 데이터에 대한 클래스입니다.

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentException | 음수 비용 값이 지정된 경우. |

### 또한보십시오

* enum [TimeUnitType](../../timeunittype/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* 네임스페이스 [Aspose.Tasks](../../timephaseddata/)
* 집회 [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
