---
title: "Calendar.GetWorkingTimes"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 메서드. 지정된 날짜에 대한 작업 시간의 WorkingTimeCollection을 반환합니다"
type: docs
weight: 240
url: /ko/net/aspose.tasks/calendar/getworkingtimes/
---
## Calendar.GetWorkingTimes method

지정된 날짜에 대한 작업 시간의 [`WorkingTimeCollection`](../../workingtimecollection/)을 반환합니다.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dt | DateTime | 작업 시간을 가져올 날짜. |

### 반환 값

[`WorkingTime`](../../workingtime/) 인스턴스의 컬렉션.

## 예제

특정 날짜에 대한 작업 시간을 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// 특정 날짜에 대한 작업 시간 가져오기
var workingTimes = calendar.GetWorkingTimes(new DateTime(2020, 4, 8, 8, 0, 0));

// 16시간이 출력됩니다
foreach (var workingTime in workingTimes)
{
    Console.WriteLine("From: " + workingTime.From);
    Console.WriteLine("To: " + workingTime.To);
}
```

### 또 보기

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


