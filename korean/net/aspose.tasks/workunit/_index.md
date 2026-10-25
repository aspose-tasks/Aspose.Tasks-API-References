---
title: "클래스 WorkUnit"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.WorkUnit 클래스. 작업 시간을 나타냅니다."
type: docs
weight: 3630
url: /ko/net/aspose.tasks/workunit/
---
## WorkUnit class

근무 시간을 나타냅니다.

```csharp
public class WorkUnit
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [WorkUnit](workunit/)(DateTime, DateTime) | `WorkUnit` 클래스의 새 인스턴스를 초기화합니다. 지정된 From 및 To 날짜로 새 WorkUnit 객체를 생성합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [From](../../aspose.tasks/workunit/from/) { get; set; } | From 날짜를 가져오거나 설정합니다. |
| [To](../../aspose.tasks/workunit/to/) { get; set; } | To 날짜를 가져오거나 설정합니다. |
| [WorkingHours](../../aspose.tasks/workunit/workinghours/) { get; set; } | 작업 시간의 기간을 가져오거나 설정합니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


