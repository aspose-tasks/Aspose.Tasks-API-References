---
title: "열거형 TaskStatus"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TaskStatus enum. 작업의 상태를 지정합니다."
type: docs
weight: 2460
url: /ko/net/aspose.tasks/taskstatus/
---
## TaskStatus enumeration

작업 상태를 지정합니다.

```csharp
public enum TaskStatus
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `-1` | 정의되지 않은 작업 상태. |
| Complete | `0` | 작업이 100% 완료되었습니다. |
| OnSchedule | `1` | 작업은 timephased 누적 완료 비율이 상태 날짜 전날까지 최소한으로 퍼져 있으면 일정에 맞습니다. |
| Late | `2` | 작업은 timephased 누적 완료 비율이 상태 날짜 전날 자정에 도달하지 않으면 지연됩니다. |
| Future | `3` | 'Future' 작업 상태는 작업 시작 날짜가 상태 날짜보다 클 때 설정됩니다. |

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


