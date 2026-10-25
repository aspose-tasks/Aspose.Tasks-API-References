---
title: "Project.SelectAllChildTasks"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。递归收集根任务的所有子任务。"
type: docs
weight: 1230
url: /zh/net/aspose.tasks/project/selectallchildtasks/
---
## Project.SelectAllChildTasks method

递归收集根任务的所有子任务。

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### 返回值

任务的集合。

## 示例

展示如何重新编号所选任务的 WBS 代码。

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

var tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// 输出：""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode(new List<int> { 1, 2, 3 });

Console.WriteLine("\nWBS codes after: ");

// 输出：""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### 另见

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


