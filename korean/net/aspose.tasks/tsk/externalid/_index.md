---
title: "Tsk.ExternalId"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업이 외부 작업인 경우 해당 작업의 외부 ID를 포함합니다."
type: docs
weight: 360
url: /ko/net/aspose.tasks/tsk/externalid/
---
## Tsk.ExternalId field

작업이 외부 작업인 경우 해당 작업의 외부 ID를 포함합니다.

```csharp
public static readonly Key<int, TaskKey> ExternalId;
```

## 예제

교차 프로젝트 작업을 식별하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "External.mpp");
var externalTask = project.RootTask.Children.GetByUid(1);

// 외부 프로젝트에서 작업의 ID 표시
Console.WriteLine(externalTask.Get(Tsk.Id).ToString());

// 원본 프로젝트에서 작업의 ID 표시
Console.WriteLine(externalTask.Get(Tsk.ExternalId).ToString());
```

교차 프로젝트 작업 링크를 만드는 방법을 보여줍니다 - 다른 (외부) 프로젝트의 작업에 대한 링크.

```csharp
Project project = new Project();
var summary = project.RootTask.Children.Add("Summary Task");

// 다른 프로젝트의 작업에 대한 링크를 만들기 위해서는
// 현재 프로젝트에 해당 작업의 복제본(또는 "외부") 작업을 생성해야 합니다.

Task t2 = summary.Children.Add("External Task");
t2.Set(Tsk.ExternalTaskProject, "ExternalProject.mpp"); // here we set path to external project's MPP file.
t2.Set(Tsk.ExternalId, 1); // Set External task's Id.
t2.Set(Tsk.ExternalUid, 2); // External task's Unique Id should be set.
t2.Set(Tsk.IsExternalTask, true);
t2.Set(Tsk.IsManual, new NullableBool(false));
t2.Set(Tsk.IsSummary, false);

Task t = summary.Children.Add("Task");
TaskLink link = project.TaskLinks.Add(t2, t);
link.IsCrossProject = true;
link.LinkType = TaskLinkType.FinishToStart;
link.CrossProjectName = "ExternalProject.mpp\\\\1"; // <- here external task's Id is used.
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


