---
title: "TaskCollection.GetByUid"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskCollection 메서드. 지정된 Uid를 가진 작업을 반환하며, 해당 작업의 상위는 이 컬렉션의 부모 작업입니다."
type: docs
weight: 80
url: /ko/net/aspose.tasks/taskcollection/getbyuid/
---
## TaskCollection.GetByUid method

이 컬렉션의 상위 작업인 조상 작업이 지정된 Uid인 작업을 반환합니다.

```csharp
public Task GetByUid(int uid)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| uid | Int32 | TaskEntity Uid. |

### 반환 값

지정된 uid를 가진 [`Task`](../../task/) 클래스의 인스턴스를 반환하며, 해당 작업의 상위는 이 컬렉션의 부모 작업입니다.

## 예제

작업 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 작업 컬렉션은 읽기 전용이 아니며 확장할 수 있습니다.
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// 작업 생성
var task1 = project.RootTask.Children.Add();
task1.Set(Tsk.Name, "Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task1.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task3.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task3.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2", 2);
task2.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// 프로젝트 작업 출력
Console.WriteLine("Count of tasks: " + project.RootTask.Children.Count);
foreach (var child in project.RootTask.Children)
{
    Console.WriteLine("Parent Project: " + project.RootTask.ParentProject.Get(Prj.Name));
    Console.WriteLine("Task name: " + child.Get(Tsk.Name));
    Console.WriteLine("Task start: " + child.Get(Tsk.Start));
    Console.WriteLine("Task duration: " + child.Get(Tsk.Duration));
    Console.WriteLine("Task finish: " + child.Get(Tsk.Finish));
    Console.WriteLine();
}

// 작업은 ID로 컬렉션에서 가져올 수 있습니다.
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// 또는 UID로
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// 또한 반복 작업을 추가할 수 있습니다.
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2020, 4, 13, 8, 0, 0),
                                                                               Finish = new DateTime(2021, 4, 13, 17, 0, 0)
                                                                           }
                                                 }
                     };

// 시퀀스의 첫 번째 작업이 반환됩니다.
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// 컬렉션을 일반 리스트로 변환할 수 있습니다.
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### 또 보기

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


