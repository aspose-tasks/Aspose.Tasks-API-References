---
title: "TaskLink.CrossProjectName"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskLink 속성. 외부 선행 프로젝트를 가져오거나 설정합니다"
type: docs
weight: 10
url: /ko/net/aspose.tasks/tasklink/crossprojectname/
---
## TaskLink.CrossProjectName property

외부 선행 프로젝트를 가져오거나 설정합니다.

```csharp
public string CrossProjectName { get; set; }
```

## 예제

교차 프로젝트 작업 링크를 찾는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "GetCrossProjectTaskLinks.mpp");

// 교차 프로젝트 작업 링크 확인
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Task Link: " + taskLink.ToString());
    if (taskLink.IsCrossProject)
    {
        Console.WriteLine(taskLink.CrossProjectName);
    }
}
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

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


