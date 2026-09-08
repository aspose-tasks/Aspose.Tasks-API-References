---
title: "ICalendar.GetTaskFinishDateFromDuration"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ICalendar 메서드. 시작 날짜의 분할 부분과 작업 기간을 기반으로 작업의 종료 날짜와 시간을 계산합니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks/icalendar/gettaskfinishdatefromduration/
---
## ICalendar.GetTaskFinishDateFromDuration method

작업의 시작 날짜, 분할 부분 및 작업 기간을 기준으로 작업 종료 날짜와 시간을 계산합니다.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 작업 | 작업 | 종료 날짜를 계산할 작업. |
| duration | TimeSpan | 계산할 기간. |

### 반환 값

주어진 시작 날짜와 기간에 대한 작업의 종료 날짜.

## 비고

작업이 요약이거나 null이거나 시작 날짜가 설정되지 않은 경우 DateTime.MinValue를 반환합니다.

### 또 보기

* class [Task](../../task/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


