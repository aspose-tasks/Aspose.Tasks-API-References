---
title: "Tsk.IgnoreResourceCalendar"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업 일정이 할당된 리소스의 캘린더를 고려하는지 여부를 결정합니다."
type: docs
weight: 530
url: /ko/net/aspose.tasks/tsk/ignoreresourcecalendar/
---
## Tsk.IgnoreResourceCalendar field

작업 일정이 해당 작업에 할당된 리소스의 캘린더를 고려하는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, TaskKey> IgnoreResourceCalendar;
```

## 예제

Tsk.IgnoreResourceCalendar 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreResourceCalendar, true);

Console.WriteLine("Ignore Resource Calendar: " + task.Get(Tsk.IgnoreResourceCalendar));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


