---
title: "Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 수동 작업을 자동 일정으로 전환할 때 가장 가까운 작업 시간에 유지해야 하는지 여부를 결정합니다."
type: docs
weight: 400
url: /ko/net/aspose.tasks/prj/keeptaskonnearestworkingtimewhenmadeautoscheduled/
---
## Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled field

수동 작업을 자동 일정으로 전환할 때 가장 가까운 작업 시간에 유지해야 하는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled;
```

## 예제

Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled, true);

Console.WriteLine("Keep Task On Nearest Working Time When Made Auto Scheduled: " + project.Get(Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


