---
title: "Prj.WeekStartDay"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 주의 첫 번째 요일"
type: docs
weight: 780
url: /ko/net/aspose.tasks/prj/weekstartday/
---
## Prj.WeekStartDay field

한 주의 첫 번째 날.

```csharp
public static readonly Key<DayType, PrjKey> WeekStartDay;
```

## 예제

프로젝트의 평일 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "WriteWeekdayProperties.mpp");

// 평일 속성을 설정합니다
project.Set(Prj.WeekStartDay, DayType.Monday);
project.Set(Prj.DaysPerMonth, 24);
project.Set(Prj.MinutesPerDay, 540);
project.Set(Prj.MinutesPerWeek, 3240);

// 평일 속성을 표시합니다
Console.WriteLine("Week Start Date: " + project.Get(Prj.WeekStartDay));
Console.WriteLine("Days Per Month: " + project.Get(Prj.DaysPerMonth));
Console.WriteLine("Minutes Per Day: " + project.Get(Prj.MinutesPerDay));
Console.WriteLine("Minutes Per Week: " + project.Get(Prj.MinutesPerWeek));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [DayType](../../daytype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


