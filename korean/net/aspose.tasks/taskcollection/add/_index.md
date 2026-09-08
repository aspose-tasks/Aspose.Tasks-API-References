---
title: "TaskCollection.Add"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskCollection 메서드. 지정된 작업을 TaskCollection 클래스의 인스턴스에 추가합니다. ParentProject.CalculationMode가 None인 경우, 이 메서드 사용 후 Project.Recalculate를 호출해야 합니다. 이 메서드는 모든 프로젝트 작업의 시작/완료 날짜를 재조정하고, 조기/후기 날짜를 설정하며, 여유시간, 작업량 및 비용 필드, ID 및 개요 수준과 같은 종속 필드를 계산합니다. ParentProject.CalculationMode가 Manual인 경우, 메서드는 작업 ID, 개요 수준 및 개요 번호만 자동으로 계산합니다. ParentProject.CalculationMode가 Automatic인 경우, 메서드는 모든 프로젝트 작업을 자동으로 재조정하고(시작/완료 날짜, 조기/후기 날짜 설정), 여유시간, 작업량 및 비용 필드를 계산하고, ID와 개요 수준을 재계산합니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

`[`TaskCollection`](../)` 클래스의 인스턴스에 지정된 작업을 추가합니다. ParentProject.CalculationMode가 None인 경우, 이 메서드 사용 후 Project.Recalculate()를 호출해야 합니다(모든 프로젝트 작업을 재조정하고(시작/완료 날짜, 조기/후기 날짜 설정) 여유시간, 작업량 및 비용 필드, ID 및 개요 수준과 같은 종속 필드를 계산합니다). ParentProject.CalculationMode가 Manual인 경우, 메서드는 작업 ID, 개요 수준 및 개요 번호만 자동으로 계산합니다. ParentProject.CalculationMode가 Automatic인 경우, 메서드는 모든 프로젝트 작업을 자동으로 재조정합니다(시작/완료 날짜, 조기/후기 날짜 설정, 여유시간, 작업량 및 비용 필드 계산, ID와 개요 수준을 재계산).

```csharp
public void Add(Task item)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 항목 | 작업 | 이 작업 컬렉션에 추가되어야 하는 지정된 작업입니다. |

## 예제

작업을 다른 상위 작업 아래로 이동하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "MoveTask.mpp") { CalculationMode = CalculationMode.Automatic };

// ID로 작업 가져오기
var task = project.RootTask.Children.GetByUid(6);
var task2 = project.RootTask.Children.GetByUid(3);

// 작업 6을 다른 상위 작업에 추가하기
task2.Children.Add(task);
```

### 또 보기

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add() {#add}

마지막 작업과 동일한 개요 수준에서 프로젝트 작업 컬렉션에 새 작업을 추가합니다.

```csharp
public Task Add()
```

### 반환 값

새로 추가된 [`Task`](../../task/) 클래스의 인스턴스를 반환합니다.

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

---

## Add(string) {#add_2}

하위 작업 컬렉션에 새 작업을 추가합니다.

```csharp
public Task Add(string taskName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| taskName | 문자열 | 지정된 작업 이름입니다. |

### 반환 값

새로 추가된 [`Task`](../../task/) 클래스의 인스턴스를 반환합니다.

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

---

## Add(string, int) {#add_3}

하위 작업 컬렉션에 새로운 반복 작업을 추가합니다.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| taskName | 문자열 | 지정된 작업 이름입니다. |
| beforeTaskId | Int32 | 새 작업이 삽입될 작업 이전의 지정된 ID입니다. |

### 반환 값

지정된 ID를 가진 작업 앞에 삽입된 작업을 반환합니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentOutOfRangeException | 지정된 ID가 유효한 작업 ID가 아닌 경우 ArgumentOutOfRangeException이 발생합니다. |

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

---

## Add(RecurringTaskParameters) {#add_1}

지정된 ID를 가진 작업 앞에 새 작업을 삽입하고 동일한 개요 수준에 배치합니다.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| parameters | RecurringTaskParameters | 반복 작업 생성을 위한 지정된 매개변수입니다. |

### 반환 값

새로 추가된 [`Task`](../../task/) 클래스의 인스턴스를 반환합니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | 지정된 매개변수가 null인 경우 발생합니다. |
| ArgumentException | 지정된 매개변수가 유효하지 않은 경우 발생합니다. |

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
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


