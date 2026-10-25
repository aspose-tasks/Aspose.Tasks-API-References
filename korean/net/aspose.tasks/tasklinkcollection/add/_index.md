---
title: "TaskLinkCollection.Add"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskLinkCollection 메서드. TaskLinkCollection 객체에 추가된 FinishStart TaskLink 인스턴스를 반환합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

Finish-Start [`TaskLink`](../../tasklink/)의 인스턴스를 반환하며, 이는 TaskLinkCollection 객체에 추가되었습니다.

```csharp
public TaskLink Add(Task pred, Task succ)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pred | 작업 | 선행 작업. |
| succ | 작업 | 후속 작업. |

### 반환 값

이 객체에 추가된 작업 링크 인스턴스.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | 입력 작업 중 하나라도 null이면 ArgumentNullException이 발생합니다. |

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
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

[`TaskLink`](../../tasklink/)의 인스턴스를 반환하며, 이는 TaskLinkCollection 객체에 추가되었습니다.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pred | 작업 | 선행 작업. |
| succ | 작업 | 후속 작업. |
| linkType | TaskLinkType | 링크 유형 [`TaskLinkType`](../../tasklinktype/) |

### 반환 값

이 객체에 추가된 작업 링크 인스턴스.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | 입력 작업 중 하나라도 null이면 ArgumentNullException이 발생합니다. |

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
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

[`TaskLink`](../../tasklink/)의 인스턴스를 반환하며, 이는 TaskLinkCollection 객체에 추가되었습니다.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pred | 작업 | 선행 작업. |
| succ | 작업 | 후속 작업. |
| linkType | TaskLinkType | 링크 유형 [`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | 링크 지연 [`Duration`](../../duration/). |

### 반환 값

이 객체에 추가된 작업 링크.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | 입력 작업 중 하나라도 null이면 ArgumentNullException이 발생합니다. |

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
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

ICollection의 Add 메서드에 대한 스텁 구현으로, NotSupportedException만 발생시킵니다.

```csharp
public void Add(TaskLink item)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 항목 | TaskLink | 추가할 항목. |

### 또 보기

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


