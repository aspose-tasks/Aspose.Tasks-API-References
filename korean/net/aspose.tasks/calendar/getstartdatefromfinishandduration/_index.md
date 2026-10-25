---
title: "Calendar.GetStartDateFromFinishAndDuration"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 메서드. 지정된 종료 날짜와 지속 시간을 기반으로 시작 날짜를 반환합니다."
type: docs
weight: 200
url: /ko/net/aspose.tasks/calendar/getstartdatefromfinishandduration/
---
## GetStartDateFromFinishAndDuration(DateTime, Duration) {#getstartdatefromfinishandduration}

지정된 종료 날짜와 기간을 기반으로 시작 날짜를 반환합니다.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, Duration duration)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 끝 | DateTime | 지정된 종료 날짜. |
| duration | Duration | 지정된 기간. |

### 반환 값

계산된 시작 날짜.

## 예제

종료 날짜와 지속 시간을 사용하여 시작 날짜를 얻는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// 종료 날짜와 지속 시간을 사용하여 시작 날짜 가져오기
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), project.GetDuration(16, TimeUnitType.Hour));

// 2020년 4월 8일 오전 9시가 출력됩니다.
Console.WriteLine(startDate);
```

### 또 보기

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetStartDateFromFinishAndDuration(DateTime, TimeSpan) {#getstartdatefromfinishandduration_1}

지정된 종료 날짜와 기간을 기반으로 시작 날짜를 반환합니다.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, TimeSpan duration)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 끝 | DateTime | 지정된 종료 날짜. |
| duration | TimeSpan | 지정된 기간. |

### 반환 값

계산된 시작 날짜.

## 예제

종료 날짜와 지속 시간(시간 간격)으로 시작 날짜를 얻는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// 종료 날짜와 지속 시간을 사용하여 시작 날짜 가져오기
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), TimeSpan.FromHours(16));

// 2020년 4월 8일 오전 9시가 출력됩니다.
Console.WriteLine(startDate);
```

### 또 보기

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


