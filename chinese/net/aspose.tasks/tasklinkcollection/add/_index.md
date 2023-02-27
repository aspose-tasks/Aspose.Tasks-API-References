---
title: TaskLinkCollection.Add
second_title: Aspose.Tasks for .NET API 参考
description: TaskLinkCollection 方法. 返回 FinishStart 的实例TaskLink已添加到 TaskLinkCollection 对象中
type: docs
weight: 40
url: /zh/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

返回 Finish-Start 的实例[`TaskLink`](../../tasklink/)已添加到 TaskLinkCollection 对象中。

```csharp
public TaskLink Add(Task pred, Task succ)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pred | Task | 前任任务。 |
| succ | Task | 继任任务。 |

### 返回值

已添加到此对象的任务链接实例。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | 如果任何输入任务等于 null，则ArgumentNullException将被抛出。 |

### 也可以看看

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* 命名空间 [Aspose.Tasks](../../tasklinkcollection/)
* 部件 [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

返回一个实例[`TaskLink`](../../tasklink/)已添加到 TaskLinkCollection 对象中。

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pred | Task | 前任任务。 |
| succ | Task | 继任任务。 |
| linkType | TaskLinkType | 链接类型[`TaskLinkType`](../../tasklinktype/) |

### 返回值

已添加到此对象的任务链接实例。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | 如果任何输入任务等于 null，则ArgumentNullException将被抛出。 |

### 也可以看看

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* 命名空间 [Aspose.Tasks](../../tasklinkcollection/)
* 部件 [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

返回一个实例[`TaskLink`](../../tasklink/)已添加到 TaskLinkCollection 对象中。

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pred | Task | 前任任务。 |
| succ | Task | 继任任务。 |
| linkType | TaskLinkType | 链接类型[`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | 链路滞后[`Duration`](../../duration/). |

### 返回值

已添加到此对象的任务链接。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | 如果任何输入任务等于 null，则ArgumentNullException将被抛出。 |

### 也可以看看

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* 命名空间 [Aspose.Tasks](../../tasklinkcollection/)
* 部件 [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

这是 ICollection 的 Add 方法的存根实现，它只抛出 NotSupportedException

```csharp
public void Add(TaskLink item)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| item | TaskLink | 要添加的项目。 |

### 也可以看看

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* 命名空间 [Aspose.Tasks](../../tasklinkcollection/)
* 部件 [Aspose.Tasks](../../../)


