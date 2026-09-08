---
title: "Project.DefaultWeekWorkingDays"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. 프로젝트 기본 주 작업일 및 작업 시간을 나타내는 WeekDayCollection 클래스의 인스턴스를 가져옵니다."
type: docs
weight: 370
url: /ko/net/aspose.tasks/project/defaultweekworkingdays/
---
## Project.DefaultWeekWorkingDays property

[`WeekDayCollection`](../../weekdaycollection/) 클래스의 인스턴스를 가져옵니다. 이는 프로젝트 기본 주 작업일 및 작업 시간의 컬렉션을 나타냅니다.

```csharp
public WeekDayCollection DefaultWeekWorkingDays { get; }
```

### 반환 값

[`WeekDayCollection`](../../weekdaycollection/) 클래스의 인스턴스로, [`WeekDay`](../../weekday/) 객체 목록을 포함합니다.

## 비고

데이터는 mpp 파일에만 포함되어 있으며 (xml에는 포함되지 않음).

## 예제

기본 주 작업일을 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2003.mpp");
foreach (var weekDay in project.DefaultWeekWorkingDays)
{
    Console.WriteLine("From: " + weekDay.FromDate);
    Console.WriteLine("From: " + weekDay.ToDate);
    Console.WriteLine("Day type: " + weekDay.DayType);
    Console.WriteLine("Is day working: " + weekDay.DayWorking);
}
```

### 또 보기

* class [WeekDayCollection](../../weekdaycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


