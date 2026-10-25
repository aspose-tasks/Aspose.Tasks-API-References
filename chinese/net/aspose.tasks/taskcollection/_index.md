---
title: "类 TaskCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TaskCollection 类。表示 Task 对象的集合"
type: docs
weight: 2390
url: /zh/net/aspose.tasks/taskcollection/
---
## TaskCollection class

表示一个 [`Task`](../task/) 对象的集合。

```csharp
public class TaskCollection : IList<Task>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | 获取 TaskCollection 中包含的对象数量。 |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读。 |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | 返回指定索引处的元素。 |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | 获取 TaskCollection 对象的父项目。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | 在与最后一个任务相同的大纲级别上向项目任务集合中添加新任务。 |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | 在具有指定 id 的任务之前插入新任务，并保持相同的大纲级别。 |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | 向子任务集合中添加新任务。 |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | 将指定任务添加到 `TaskCollection` 类的实例中。如果 ParentProject.CalculationMode 为 None，用户应在使用此方法后调用 Project.Recalculate()（它将重新安排所有项目任务（开始/结束日期，设置提前/延后日期）并计算诸如空闲时间、工作和成本字段、ID 和大纲级别等依赖字段）。如果 ParentProject.CalculationMode 为 Manual，方法仅自动计算任务 ID、大纲级别和大纲编号。如果 ParentProject.CalculationMode 为 Automatic，方法会自动重新安排所有项目任务（开始/结束日期，设置提前/延后日期，计算空闲时间、工作和成本字段，重新计算 ID 和大纲级别）。 |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | 向子任务集合中添加新的循环任务。 |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | 检查集合是否包含指定项。 |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | 返回具有指定 Id 且其祖先是此集合的父任务的任务。 |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | 返回具有指定 Uid 且其祖先是此集合的父任务的任务。 |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | 这是 IList 的 Insert 方法的存根实现，仅抛出 NotSupportedException。 |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | 这是 ICollection 的 Remove 方法的存根实现，仅抛出 NotSupportedException。 |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | 将 TaskCollection 对象转换为 [`Task`](../task/) 对象的列表。 |

## 示例

展示如何使用任务集合。

```csharp
var project = new Project();

// 任务集合不是只读的，可以扩展
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// 创建任务
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

// 打印项目任务
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

// 可以通过 ID 从集合中获取任务
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// 或通过 UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// 也可以添加循环任务
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

// 返回序列中的第一个任务
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// 集合可以转换为普通列表
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### 另见

* class [Task](../task/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


