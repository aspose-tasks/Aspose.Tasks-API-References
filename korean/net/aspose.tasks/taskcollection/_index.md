---
title: "클래스 TaskCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TaskCollection 클래스. Task 객체의 컬렉션을 나타냅니다"
type: docs
weight: 2390
url: /ko/net/aspose.tasks/taskcollection/
---
## TaskCollection class

[`Task`](../task/) 객체의 컬렉션을 나타냅니다.

```csharp
public class TaskCollection : IList<Task>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | TaskCollection에 포함된 객체 수를 가져옵니다. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | 지정된 인덱스의 요소를 반환합니다. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | TaskCollection 객체의 상위 프로젝트를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | 마지막 작업과 동일한 개요 수준에서 프로젝트 작업 컬렉션에 새 작업을 추가합니다. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | 지정된 ID를 가진 작업 앞에 새 작업을 삽입하고 동일한 개요 수준에 배치합니다. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | 하위 작업 컬렉션에 새 작업을 추가합니다. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | `TaskCollection` 클래스의 인스턴스에 지정된 작업을 추가합니다. ParentProject.CalculationMode가 None인 경우, 이 메서드 사용 후에 Project.Recalculate()를 호출해야 합니다(모든 프로젝트 작업(시작/종료 날짜)을 재조정하고 조기/지연 날짜를 설정하며, 여유시간, 작업 및 비용 필드, ID 및 개요 수준과 같은 종속 필드를 계산합니다). ParentProject.CalculationMode가 Manual인 경우, 메서드는 작업 ID, 개요 수준 및 개요 번호만 자동으로 계산합니다. ParentProject.CalculationMode가 Automatic인 경우, 메서드는 모든 프로젝트 작업을 자동으로 재조정합니다(시작/종료 날짜, 조기/지연 날짜 설정, 여유시간, 작업 및 비용 필드 계산, ID 및 개요 수준 재계산). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | 하위 작업 컬렉션에 새로운 반복 작업을 추가합니다. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | 컬렉션에 지정된 항목이 포함되어 있는지 확인합니다. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | 이 컬렉션의 상위 작업인 조상 작업이 지정된 Id인 작업을 반환합니다. |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | 이 컬렉션의 상위 작업인 조상 작업이 지정된 Uid인 작업을 반환합니다. |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | IList의 Insert 메서드에 대한 스텁 구현으로, NotSupportedException만 발생시킵니다. |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | ICollection의 Remove 메서드에 대한 스텁 구현으로, NotSupportedException만 발생시킵니다. |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | TaskCollection 객체를 [`Task`](../task/) 객체 목록으로 변환합니다. |

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

* class [Task](../task/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


