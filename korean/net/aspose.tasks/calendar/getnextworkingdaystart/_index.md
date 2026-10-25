---
title: "Calendar.GetNextWorkingDayStart"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 메서드. 지정된 날짜에 대한 다음 근무일 시작 시간을 계산합니다"
type: docs
weight: 180
url: /ko/net/aspose.tasks/calendar/getnextworkingdaystart/
---
## Calendar.GetNextWorkingDayStart method

지정된 날짜에 대한 다음 작업일 시작 시간을 계산합니다.

```csharp
public DateTime GetNextWorkingDayStart(DateTime date)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 날짜 | DateTime | 다음 근무일 시작 시간을 구할 날짜. |

### 반환 값

다음 근무일 시작 DateTime.

## 예제

캘린더를 사용하여 다음 근무일 시작 시간을 얻는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// 다음 근무일 시작 시간 가져오기 (주말은 건너뜁니다)
var nextWorkingDayStart = calendar.GetNextWorkingDayStart(new DateTime(2020, 4, 10, 13, 0, 0));

// 2020년 4월 13일 오전 9시가 출력됩니다.
Console.WriteLine(nextWorkingDayStart);
```

### 또 보기

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


