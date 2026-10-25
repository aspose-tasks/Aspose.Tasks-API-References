---
title: "CalendarCollection.Add"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarCollection 메서드. 이 CalendarCollection 객체에 새 기본 캘린더를 추가하고 추가된 캘린더를 반환합니다"
type: docs
weight: 20
url: /ko/net/aspose.tasks/calendarcollection/add/
---
## Add(string) {#add}

이 CalendarCollection 객체에 새 기본 캘린더를 추가하고 추가된 캘린더를 반환합니다.

```csharp
public Calendar Add(string name)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | 문자열 | 캘린더 이름. |

### 반환 값

추가된 [`Calendar`](../../calendar/) 객체.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentException | 캘린더 이름이 null인 경우 발생합니다. |

## 예제

표준 캘린더를 만드는 방법을 보여줍니다

```csharp
var project = new Project();

// 캘린더를 정의하고 표준으로 만듭니다
var calendar = project.Calendars.Add("New Standard Calendar");
Calendar.MakeStandardCalendar(calendar);

project.Save(OutDir + "MakeAStandardCalendar_out.xml", SaveFileFormat.Xml);
```

### 또 보기

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, Calendar) {#add_1}

지정된 기본 캘린더와 함께 새 캘린더를 이 CalendarCollection 객체에 추가하고 추가된 캘린더를 반환합니다.

```csharp
public Calendar Add(string name, Calendar baseCalendar)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | 문자열 | 지정된 이름. |
| baseCalendar | Calendar | 지정된 기본 캘린더. |

### 반환 값

추가된 [`Calendar`](../../calendar/) 객체.

## 예제

새 캘린더를 추가하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 새 캘린더는 컬렉션의 Add 오버로드를 사용하여 프로젝트의 캘린더 컬렉션에 추가할 수 있습니다.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### 또 보기

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


