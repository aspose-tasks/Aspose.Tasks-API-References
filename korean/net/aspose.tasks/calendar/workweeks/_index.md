---
title: "Calendar.WorkWeeks"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 속성. WorkWeekCollections 객체를 가져옵니다. 캘린더와 연결된 작업 주의 컬렉션입니다."
type: docs
weight: 130
url: /ko/net/aspose.tasks/calendar/workweeks/
---
## Calendar.WorkWeeks property

WorkWeekCollections 객체를 가져옵니다. 캘린더와 연결된 작업 주 컬렉션입니다.

```csharp
public WorkWeekCollection WorkWeeks { get; }
```

## 예제

작업 주 정보를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "WorkWithWorkWeekCollection.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var workWeek in calendar.WorkWeeks)
{
    // 작업 주 이름, 시작 및 종료 날짜 표시
    var name = workWeek.Name;
    var fromDate = workWeek.FromDate;
    var toDate = workWeek.ToDate;
    Console.WriteLine("Name: " + name);
    Console.WriteLine("From Date: " + fromDate);
    Console.WriteLine("To Date: " + toDate);

    // 이 데이터는 "Details." 버튼과 관련된 것으로, 특정 요일에 특수 작업 시간을 설정하거나 비작업으로 만들 수 있습니다.
    foreach (var day in workWeek.WeekDays)
    {
        // 작업 시간을 추가로 탐색하고 이를 표시할 수 있습니다.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}
```

### 또 보기

* class [WorkWeekCollection](../../workweekcollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


