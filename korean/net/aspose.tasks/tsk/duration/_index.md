---
title: "Tsk.Duration"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 시작 날짜, 종료 날짜, 캘린더 및 기타 일정 요소를 기반으로 Microsoft Project에서 입력되거나 계산된 작업의 전체 활성 작업 시간 범위입니다."
type: docs
weight: 300
url: /ko/net/aspose.tasks/tsk/duration/
---
## Tsk.Duration field

시작 날짜, 종료 날짜, 캘린더 및 기타 일정 요소를 기반으로 Microsoft Project에서 입력되거나 계산된 작업의 전체 활성 작업 시간 범위.

```csharp
public static readonly Key<Duration, TaskKey> Duration;
```

## 예제

작업의 지속 시간을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddTaskDuration_out.xml", SaveFileFormat.Xml);
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


