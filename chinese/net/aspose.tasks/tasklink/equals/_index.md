---
title: "TaskLink.Equals"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskLink 方法。返回一个值，指示此实例是否等于指定的对象"
type: docs
weight: 90
url: /zh/net/aspose.tasks/tasklink/equals/
---
## Equals(TaskLink) {#equals}

返回一个值，指示此实例是否等于指定的对象。

```csharp
public bool Equals(TaskLink other)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | TaskLink | 要与此实例比较的指定的 [`TaskLink`](../) 类实例。 |

### 返回值

**True** if the specified instance of the [`TaskLink`](../) class has the same predecessor and successor tasks as this instance; otherwise, **false**.

## 示例

展示如何检查任务链接的相等性。

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// 任务链接的相等性基于前置任务和后续任务。
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### 另见

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

返回一个值，指示此实例是否等于指定的对象。

```csharp
public override bool Equals(object obj)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | 对象 | 与此实例比较的对象。 |

### 返回值

**True** if the specified object is a TaskLink that has the same predecessor and successor as this instance; otherwise, **false**.

## 示例

展示如何检查任务链接的相等性。

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// 任务链接的相等性基于前置任务和后续任务。
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### 另见

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


