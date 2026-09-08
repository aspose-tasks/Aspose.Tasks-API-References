---
title: "Calendar.GetWorkingHours"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 메서드. 지정된 날짜 시간 구간에 대한 작업 단위, 시작, 종료 및 작업 시간의 기간을 반환합니다."
type: docs
weight: 220
url: /ko/net/aspose.tasks/calendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

지정된 날짜 시간 구간에 대한 작업 단위 - 시작, 종료 및 작업 시간 지속 시간을 반환합니다.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | DateTime | 구간의 시작 날짜. |
| 끝 | DateTime | 구간의 종료 날짜. |

### 반환 값

[`WorkUnit`](../../workunit/) 클래스의 인스턴스로, 작업 시간의 시작, 종료 및 기간을 포함합니다.

## 예제

특정 날짜에 대한 작업 시간을 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// 특정 날짜에 대한 작업 시간을 가져옵니다.
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

// 16시간이 출력됩니다
Console.WriteLine(workUnit.WorkingHours);
```

### 또 보기

* class [WorkUnit](../../workunit/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

지정된 날짜의 작업 시간 양을 반환합니다.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dt | DateTime | 작업 시간을 가져올 날짜. |

### 반환 값

지정된 날짜의 작업 시간.

## 예제

특정 날짜에 대한 작업 시간을 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// 특정 날짜에 대한 작업 시간을 가져옵니다.
var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 10));

// 8시간이 출력됩니다
Console.WriteLine(workingHours.Hours);
```

### 또 보기

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


