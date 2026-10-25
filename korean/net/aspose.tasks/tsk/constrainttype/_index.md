---
title: "Tsk.ConstraintType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업 일정에 적용할 수 있는 제약 유형에 대한 선택지를 제공합니다."
type: docs
weight: 210
url: /ko/net/aspose.tasks/tsk/constrainttype/
---
## Tsk.ConstraintType field

작업 일정에 적용할 수 있는 제약 유형에 대한 선택지를 제공합니다.

```csharp
public static readonly Key<ConstraintType, TaskKey> ConstraintType;
```

## 예제

작업에 대한 제약을 가져오거나 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ConstraintAsLateAsPossible.mpp");

// ID가 11인 작업에 대해 가능한 한 늦게 제약을 설정합니다.
var newTask = project.RootTask.Children.GetById(11);
newTask.Set(Tsk.ConstraintType, ConstraintType.AsLateAsPossible);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 수집된 모든 작업을 파싱합니다
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.ConstraintType).ToString());
    Console.WriteLine(task.Get(Tsk.ConstraintDate).ToShortDateString() == "1/1/2000" ? "NA" : task.Get(Tsk.ConstraintDate).ToShortDateString());
}

SaveOptions options = new PdfSaveOptions
{
    StartDate = project.Get(Prj.StartDate),
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "SetConstraintAsLateAsPossible_out.pdf", options);
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ConstraintType](../../constrainttype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


