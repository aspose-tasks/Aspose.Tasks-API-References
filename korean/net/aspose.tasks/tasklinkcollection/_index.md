---
title: "클래스 TaskLinkCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TaskLinkCollection 클래스. Task 객체의 컬렉션을 나타냅니다."
type: docs
weight: 2420
url: /ko/net/aspose.tasks/tasklinkcollection/
---
## TaskLinkCollection class

[`Task`](../task/) 객체의 컬렉션을 나타냅니다.

```csharp
public class TaskLinkCollection : IList<TaskLink>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/tasklinkcollection/count/) { get; } | `TaskLinkCollection` 객체에 포함된 객체 수를 가져옵니다. |
| [Item](../../aspose.tasks/tasklinkcollection/item/) { get; set; } | 지정된 인덱스에 있는 요소를 반환하거나 설정합니다. |
| [ParentProject](../../aspose.tasks/tasklinkcollection/parentproject/) { get; } | ResourceAssignmentCollection 객체의 상위 프로젝트를 가져옵니다. 이 객체의 상위 [`Project`](../project/)입니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_3)(TaskLink) | ICollection의 Add 메서드에 대한 스텁 구현으로, NotSupportedException만 발생시킵니다. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add)(Task, Task) | TaskLinkCollection 객체에 추가된 Finish-Start [`TaskLink`](../tasklink/) 인스턴스를 반환합니다. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_1)(Task, Task, TaskLinkType) | TaskLinkCollection 객체에 추가된 [`TaskLink`](../tasklink/) 인스턴스를 반환합니다. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_2)(Task, Task, TaskLinkType, Duration) | TaskLinkCollection 객체에 추가된 [`TaskLink`](../tasklink/) 인스턴스를 반환합니다. |
| [GetEnumerator](../../aspose.tasks/tasklinkcollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [Remove](../../aspose.tasks/tasklinkcollection/remove/)(TaskLink) | 프로젝트에서 작업 링크를 제거합니다. |
| [ToList](../../aspose.tasks/tasklinkcollection/tolist/)() | TaskLinkCollection 객체를 [`TaskLink`](../tasklink/) 객체 목록으로 변환합니다. |

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

* class [TaskLink](../tasklink/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


