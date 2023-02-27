---
title: TaskCollection.Add
second_title: Aspose.Tasks for .NET API 参考
description: TaskCollection 方法. 将指定任务添加到实例中TaskCollectionclass. 如果 ParentProject.CalculationMode 为 None用户应在使用此方法后调用 Project.Recalculate它将重新安排所有项目任务开始/结束日期设置早/晚日期并计算相关字段例如 slackswork和成本字段ID 和大纲级别 如果 ParentProject.CalculationMode 是手动的该方法将仅自动计算任务 ID大纲级别和大纲编号 如果 ParentProject.CalculationMode 是自动的该方法将自动重新安排所有项目的任务 开始/完成日期设置早/晚日期计算松弛时间工作和成本字段重新计算 ID 和大纲级别
type: docs
weight: 50
url: /zh/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

将指定任务添加到实例中[`TaskCollection`](../)class. 如果 ParentProject.CalculationMode 为 None，用户应在使用此方法后调用 Project.Recalculate()（它将重新安排所有项目任务（开始/结束日期，设置早/晚日期）并计算相关字段，例如 slacks、work和成本字段、ID 和大纲级别）。 如果 ParentProject.CalculationMode 是手动的，该方法将仅自动计算任务 ID、大纲级别和大纲编号。 如果 ParentProject.CalculationMode 是自动的，该方法将自动重新安排所有项目的任务 （开始/完成日期，设置早/晚日期，计算松弛时间，工作和成本字段，重新计算 ID 和大纲级别）。

```csharp
public void Add(Task item)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| item | Task | 应添加到此任务集合中的指定任务。 |

### 也可以看看

* class [Task](../../task/)
* class [TaskCollection](../)
* 命名空间 [Aspose.Tasks](../../taskcollection/)
* 部件 [Aspose.Tasks](../../../)

---

## Add() {#add}

将新任务添加到与上一个任务相同的大纲级别的项目任务集合。

```csharp
public Task Add()
```

### 返回值

返回新添加的实例[`Task`](../../task/)班级。

### 也可以看看

* class [Task](../../task/)
* class [TaskCollection](../)
* 命名空间 [Aspose.Tasks](../../taskcollection/)
* 部件 [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

向子任务集合添加新任务。

```csharp
public Task Add(string taskName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| taskName | String | 指定的任务名称。 |

### 返回值

返回新添加的实例[`Task`](../../task/)班级。

### 也可以看看

* class [Task](../../task/)
* class [TaskCollection](../)
* 命名空间 [Aspose.Tasks](../../taskcollection/)
* 部件 [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

将新的循环任务添加到子任务集合中。

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| taskName | String | 指定的任务名称。 |
| beforeTaskId | Int32 | 任务的指定 ID，将在其之前插入新任务。 |

### 返回值

返回插入到具有指定 ID 的任务之前的任务。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentOutOfRangeException | 如果指定的 ID 不是有效的任务 ID，则抛出 ArgumentOutOfRangeException。 |

### 也可以看看

* class [Task](../../task/)
* class [TaskCollection](../)
* 命名空间 [Aspose.Tasks](../../taskcollection/)
* 部件 [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

在具有指定 id 且在同一大纲级别的任务之前插入一个新任务。

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| parameters | RecurringTaskParameters | parameters 为创建周期性任务指定的参数。 |

### 返回值

返回新添加的实例[`Task`](../../task/)班级。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | 如果指定的参数为空则抛出。 |
| ArgumentException | 如果指定的参数无效则抛出。 |

### 也可以看看

* class [Task](../../task/)
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* 命名空间 [Aspose.Tasks](../../taskcollection/)
* 部件 [Aspose.Tasks](../../../)


