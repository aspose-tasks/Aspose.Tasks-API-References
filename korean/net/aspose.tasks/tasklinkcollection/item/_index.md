---
title: "TaskLinkCollection.Item"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskLinkCollection 속성. 지정된 인덱스의 요소를 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/tasklinkcollection/item/
---
## TaskLinkCollection indexer

지정된 인덱스에 있는 요소를 반환하거나 설정합니다.

```csharp
public TaskLink this[int index] { get; set; }
```

| 매개변수 | 설명 |
| --- | --- |
| 인덱스 | 가져오거나 설정할 요소의 0부터 시작하는 인덱스. |

### 반환 값

지정된 인덱스의 요소.

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


