---
title: Task
second_title: Aspose.Tasks for .NET API 参考
description: 表示项目中的任务
type: docs
weight: 2060
url: /zh/net/aspose.tasks/task/
---
## Task class

表示项目中的任务。

```csharp
public class Task : IEquatable<Task>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Assignments](../../aspose.tasks/task/assignments) { get; } | 获取此对象的资源分配集合。 |
| [Baselines](../../aspose.tasks/task/baselines) { get; set; } | 获取或设置任务基线值的集合。 |
| [Children](../../aspose.tasks/task/children) { get; } | 获取此对象的子任务集合。 代表子任务的 TaskCollection 对象。 |
| [ExtendedAttributes](../../aspose.tasks/task/extendedattributes) { get; } | 获取包含扩展属性值的 ExtendedAttributeCollection 对象。 |
| [OutlineCodes](../../aspose.tasks/task/outlinecodes) { get; set; } | 获取或设置[`OutlineCodeCollection`](../outlinecodecollection)对象. |
| [ParentProject](../../aspose.tasks/task/parentproject) { get; } | 获取任务的父项目。 |
| [ParentTask](../../aspose.tasks/task/parenttask) { get; } | 获取任务的父任务。 |
| [Predecessors](../../aspose.tasks/task/predecessors) { get; } | 得到一个[`TaskCollection`](../taskcollection)包含此任务对象的所有前辈的对象。 |
| [RecurringInfo](../../aspose.tasks/task/recurringinfo) { get; } | 获取实例[`RecurringTaskInfo`](../recurringtaskinfo)重复任务的任务的类；如果任务不是重复任务，则返回 null; 实例的信息[`RecurringTaskInfo`](../recurringtaskinfo)仅以 mpp 文件格式存在。 |
| [SplitParts](../../aspose.tasks/task/splitparts) { get; } | 获取表示任务部分的 SplitPart 集合。 |
| [Successors](../../aspose.tasks/task/successors) { get; } | 得到一个[`TaskCollection`](../taskcollection)包含此任务对象的所有后继者的对象。 |
| [TimephasedData](../../aspose.tasks/task/timephaseddata) { get; set; } | 获取或设置此任务的 TimephasedDataCollection 对象。 与任务关联的时间分段数据块。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Clone](../../aspose.tasks/task/clone)() | 创建没有子任务的任务的完整副本。 |
| [Delete](../../aspose.tasks/task/delete)() | 从父项目任务集合中删除任务及其所有分配。 |
| override [Equals](../../aspose.tasks/task/equals#equals_1)(object) | 返回一个值，指示此实例是否等于指定对象。 |
| [Equals](../../aspose.tasks/task/equals#equals)(Task) | 返回一个值，指示此实例是否等于指定的任务。 |
| [Get&lt;T&gt;](../../aspose.tasks/task/get)(Key&lt;T, TaskKey&gt;) | 返回此容器中属性映射到的值。 |
| override [GetHashCode](../../aspose.tasks/task/gethashcode)() | 返回此任务的哈希码值。 |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata)(DateTime, DateTime) | 返回[`TimephasedDataCollection`](../timephaseddatacollection)对象与[`TimephasedData`](./timephaseddata)给定开始日期和结束日期内的值。 |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata_1)(DateTime, DateTime, TimephasedDataType) | 返回[`TimephasedDataCollection`](../timephaseddatacollection)对象与[`TimephasedData`](./timephaseddata)指定时间分段数据类型的给定开始和结束日期内的值。 |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling_1)(int) | 将当前任务移动到具有指定 Id 的任务之前的同一大纲级别。 如果 ParentProject.CalculationMode 为 None 用户应在使用此方法后调用 Project.Recalculate()设置早/晚日期）并计算相关字段，例如时差、工作和成本字段、大纲级别）。 如果 ParentProject.CalculationMode 为 Manual，该方法将仅自动计算任务 ID、大纲级别和大纲编号。 如果 ParentProject。 CalculationMode 是 Automatic，该方法自动重新安排所有项目的任务 （开始/完成日期，设置早/晚日期，计算时间差、工作和成本字段，重新计算 ID 和大纲级别）。 |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling)(Task) | 将当前任务移动到指定任务之前的同一大纲级别。 如果 ParentProject.CalculationMode 为 None 用户应在使用此方法后调用 Project.Recalculate() （它将重新安排所有项目任务（开始/结束日期，提前设置/延迟日期）并计算相关字段，例如时差、工作和成本字段、大纲级别）。 如果 ParentProject.CalculationMode 为 Manual，该方法将仅自动计算任务 ID、大纲级别和大纲编号。 如果 ParentProject.CalculationMode 为 Automatic该方法自动重新安排所有项目的任务 （开始/完成日期，设置早/晚日期，计算时间差，工作和成本字段，重新计算ID和大纲级别）。 |
| [OutlineIndent](../../aspose.tasks/task/outlineindent)() | 在大纲中缩进任务。 |
| [OutlineOutdent](../../aspose.tasks/task/outlineoutdent)() | 提升大纲中的任务。 |
| [SelectAllChildTasks](../../aspose.tasks/task/selectallchildtasks)() | 递归收集该任务的所有子任务 |
| [Set&lt;T&gt;](../../aspose.tasks/task/set)(Key&lt;T, TaskKey&gt;, T) | 将指定属性映射到此容器中的指定值。 |
| override [ToString](../../aspose.tasks/task/tostring)() | 返回任务的短字符串表示。 表示的确切细节未指定，可能会发生变化。 |

### 评论

这 **任务**代表一个原子的工作。

一个可以使用 **任务**通过创建任务来规划项目并为其分配适当的资源。 项目中的任务被组织为一个有根的层次树结构，具有一个根任务和子任务的子树。

要构建任务树，可以使用专门的集合[`TaskCollection`](../taskcollection)通过访问[`RootTask`](../project/roottask)属性例如：

```csharp
Project project = new Project();

// 添加新任务
Task task1 = project.RootTask.Children.Add(); // 添加一个空名称的父任务
Task childTask1 = task1.Children.Add("Child 1");
childTask1.Set(Tsk.Start, new DateTime(2020, 2, 12, 8, 0, 0))
childTask1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask1.Set(Tsk.Finish, new DateTime(2020, 2, 12, 17, 0, 0));
Task childTask3 = task1.Children.Add("Child 3");
childTask3.Set(Tsk.Start, new DateTime(2020, 2, 13, 8, 0, 0))
childTask3.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask3.Set(Tsk.Finish, new DateTime(2020, 2, 13, 17, 0, 0));
Task childTask2 = task1.Children.Add("Child 2", 2); // 在 childTask3 之前插入一个任务
childTask2.Set(Tsk.Start, new DateTime(2020, 2, 14, 8, 0, 0))
childTask2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask2.Set(Tsk.Finish, new DateTime(2020, 2, 14, 17, 0, 0));

// 以其中一种可用格式保存项目
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

### 也可以看看

* 命名空间 [Aspose.Tasks](../../aspose.tasks)
* 部件 [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
