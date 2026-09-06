---
title: "TaskLinkCollection.Add"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskLinkCollection 方法。返回已添加到 TaskLinkCollection 对象的 FinishStart TaskLink 实例"
type: docs
weight: 40
url: /zh/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

返回已添加到 TaskLinkCollection 对象的 Finish-Start [`TaskLink`](../../tasklink/) 实例。

```csharp
public TaskLink Add(Task pred, Task succ)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 前置 | 任务 | 前置任务。 |
| 后置 | 任务 | 后置任务。 |

### 返回值

已添加到此对象的任务链接实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | 如果任意输入任务为 null，则会抛出 ArgumentNullException。 |

## 示例

展示如何使用任务链接集合。

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// 获取任务
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// 链接任务
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// 打印任务之间的链接
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// 通过索引访问编辑链接
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// 移除所有任务链接
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### 另见

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

返回已添加到 TaskLinkCollection 对象的 [`TaskLink`](../../tasklink/) 实例。

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 前置 | 任务 | 前置任务。 |
| 后置 | 任务 | 后置任务。 |
| linkType | TaskLinkType | 链接类型 [`TaskLinkType`](../../tasklinktype/) |

### 返回值

已添加到此对象的任务链接实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | 如果任意输入任务为 null，则会抛出 ArgumentNullException。 |

## 示例

展示如何使用任务链接集合。

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// 获取任务
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// 链接任务
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// 打印任务之间的链接
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// 通过索引访问编辑链接
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// 移除所有任务链接
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### 另见

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

返回已添加到 TaskLinkCollection 对象的 [`TaskLink`](../../tasklink/) 实例。

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 前置 | 任务 | 前置任务。 |
| 后置 | 任务 | 后置任务。 |
| linkType | TaskLinkType | 链接类型 [`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | 链接延迟 [`Duration`](../../duration/)。 |

### 返回值

已添加到此对象的任务链接。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | 如果任意输入任务为 null，则会抛出 ArgumentNullException。 |

## 示例

展示如何使用任务链接集合。

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// 获取任务
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// 链接任务
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// 打印任务之间的链接
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// 通过索引访问编辑链接
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// 移除所有任务链接
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### 另见

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

这是 ICollection 的 Add 方法的存根实现，只会抛出 NotSupportedException。

```csharp
public void Add(TaskLink item)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | TaskLink | 要添加的项。 |

### 另见

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


