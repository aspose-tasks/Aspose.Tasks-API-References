---
title: "TaskLinkCollection.Remove"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskLinkCollection 메서드. 프로젝트에서 작업 링크를 제거합니다."
type: docs
weight: 60
url: /ko/net/aspose.tasks/tasklinkcollection/remove/
---
## TaskLinkCollection.Remove method

프로젝트에서 작업 링크를 제거합니다.

```csharp
public bool Remove(TaskLink item)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 항목 | TaskLink | 제거할 TaskLink. |

### 반환 값

제거된 TaskLink.

## 예제

작업 링크 컬렉션 작업 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// 작업 가져오기
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// 작업 연결
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// 작업 간의 링크를 출력합니다
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// 인덱스 접근으로 링크 편집
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// 모든 작업 링크 제거
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### 또 보기

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


