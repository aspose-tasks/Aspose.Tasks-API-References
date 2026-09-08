---
title: "Calendar.GetPreviousWorkingDayEnd"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 메서드. 지정된 날짜로부터 이전 근무일의 종료 시간을 계산합니다."
type: docs
weight: 190
url: /ko/net/aspose.tasks/calendar/getpreviousworkingdayend/
---
## Calendar.GetPreviousWorkingDayEnd method

지정된 날짜로부터 이전 작업일의 종료 시간을 계산합니다.

```csharp
public DateTime GetPreviousWorkingDayEnd(DateTime date)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 날짜 | DateTime | 이전 작업 날짜 종료 시간을 계산할 날짜. |

### 반환 값

이전 작업일 종료 시점.

## 예제

캘린더를 사용하여 이전 근무일 종료 시간을 얻는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// 이전 근무일 종료 시간 가져오기
var previousWorkingDayEnd = calendar.GetPreviousWorkingDayEnd(new DateTime(2020, 4, 10, 13, 0, 0));

// 2020년 4월 9일 오후 6시가 출력됩니다.
Console.WriteLine(previousWorkingDayEnd);
```

### 또 보기

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


