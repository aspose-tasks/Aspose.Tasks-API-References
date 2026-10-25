---
title: "WorkUnit.WorkUnit"
second_title: "Aspose.Tasks for .NET API 참조"
description: "WorkUnit 생성자. WorkUnit 클래스의 새 인스턴스를 초기화합니다. 지정된 From 및 To 날짜로 새 WorkUnit 객체를 생성합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/workunit/workunit/
---
## WorkUnit constructor

[`WorkUnit`](../) 클래스의 새 인스턴스를 초기화합니다. 지정된 From 및 To 날짜로 새 WorkUnit 객체를 생성합니다.

```csharp
public WorkUnit(DateTime from, DateTime to)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| from | DateTime | 근무 시간의 시작 날짜. |
| 까지 | DateTime | 근무 시간의 종료 날짜. |

## 예제

작업 단위 정보를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// 특정 날짜에 대한 작업 시간을 가져옵니다.
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

Console.WriteLine("From: " + workUnit.From);
Console.WriteLine("To: " + workUnit.To);
Console.WriteLine("Working hours: " + workUnit.WorkingHours);
```

### 또 보기

* class [WorkUnit](../)
* namespace [Aspose.Tasks](../../workunit/)
* assembly [Aspose.Tasks](../../../)


