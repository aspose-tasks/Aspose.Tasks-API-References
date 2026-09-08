---
title: "WorkUnit.WorkingHours"
second_title: "Aspose.Tasks for .NET API 참조"
description: "WorkUnit 속성. 근무 시간의 기간을 가져오거나 설정합니다"
type: docs
weight: 40
url: /ko/net/aspose.tasks/workunit/workinghours/
---
## WorkUnit.WorkingHours property

작업 시간의 기간을 가져오거나 설정합니다.

```csharp
public TimeSpan WorkingHours { get; set; }
```

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


