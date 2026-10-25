---
title: "Prj.ScheduleFromStart"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 시작 날짜부터 프로젝트 일정을 앞쪽으로 계산할지 여부를 결정합니다"
type: docs
weight: 630
url: /ko/net/aspose.tasks/prj/schedulefromstart/
---
## Prj.ScheduleFromStart field

시작 날짜부터 프로젝트 일정을 앞쪽으로 계산할지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> ScheduleFromStart;
```

## 예제

프로젝트를 시작 날짜가 아니라 종료 날짜부터 다시 일정 잡는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.ScheduleFromStart, false);
project.Set(Prj.FinishDate, new DateTime(2020, 1, 1));

// 이제 모든 작업 날짜(Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish)가 계산됩니다. 임계 경로를 얻으려면 여유 시간을 계산해야 합니다(별도의 스레드에서 호출할 수 있지만 모든 조기/지연 날짜 계산 후에만 가능합니다).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


