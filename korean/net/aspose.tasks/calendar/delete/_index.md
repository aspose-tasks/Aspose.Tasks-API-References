---
title: "Calendar.Delete"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 메서드. 프로젝트에서 캘린더를 제거합니다."
type: docs
weight: 140
url: /ko/net/aspose.tasks/calendar/delete/
---
## Calendar.Delete method

프로젝트에서 캘린더를 제거합니다.

```csharp
public void Delete()
```

## 예제

프로젝트에서 캘린더를 삭제하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "BrokenCalendar.mpp");

// 이름으로 캘린더 가져오기
var calendar = project.Calendars.GetByName("Broken Calendar");

// 캘린더를 삭제합니다
calendar.Delete();
```

### 또 보기

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


