---
title: "Calendar.GetFinishDateByStartAndWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 메서드. 캘린더에 따라 지정된 작업 시간이 경과하는 날짜를 계산합니다."
type: docs
weight: 160
url: /ko/net/aspose.tasks/calendar/getfinishdatebystartandwork/
---
## GetFinishDateByStartAndWork(DateTime, Duration) {#getfinishdatebystartandwork}

캘린더에 따라 지정된 작업 시간이 경과하는 날짜를 계산합니다.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, Duration work)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | DateTime | 시작 날짜. |
| work | Duration | 작업 기간. |

### 반환 값

종료 날짜.

## 예제

캘린더 인스턴스를 사용하여 시작 날짜와 작업량으로 종료 날짜를 계산하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// 표준 캘린더를 사용하여 종료 날짜 계산
var finish = calendar.GetFinishDateByStartAndWork(start, work);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### 또 보기

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetFinishDateByStartAndWork(DateTime, TimeSpan) {#getfinishdatebystartandwork_1}

캘린더에 따라 지정된 작업 시간이 경과하는 날짜를 계산합니다.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, TimeSpan work)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | DateTime | 시작 날짜. |
| work | TimeSpan | 작업 기간. |

### 반환 값

종료 날짜.

## 예제

캘린더 인스턴스를 사용하여 시작 날짜와 작업(시간 간격)으로 종료 날짜를 계산하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// 표준 캘린더를 사용하여 종료 날짜 계산
var finish = calendar.GetFinishDateByStartAndWork(start, work.TimeSpan);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### 또 보기

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


