---
title: "Project.RenumberWBSCode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。重新编号所有任务的 WBS 代码。"
type: docs
weight: 1180
url: /zh/net/aspose.tasks/project/renumberwbscode/
---
## RenumberWBSCode() {#renumberwbscode}

重新编号所有任务的 WBS 代码。

```csharp
public void RenumberWBSCode()
```

## 示例

展示如何重新编号任务的 WBS 代码。

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

IEnumerable<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// 输出：""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode();

Console.WriteLine("\nWBS codes after: ");

// 输出：""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## RenumberWBSCode(List&lt;int&gt;) {#renumberwbscode_1}

重新编号已通过任务的 WBS 代码。

```csharp
public void RenumberWBSCode(List<int> taskIds)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| taskIds | List`1 | 用于重新编号 WBS 代码的任务标识符。 |

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

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


