---
title: "ChildTasksCollector"
second_title: "Aspose.Tasks for Java API 参考"
description: "收集所有子任务。"
type: docs
weight: 49
url: /zh/java/com.aspose.tasks/childtaskscollector/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.TreeAlgorithmBase
```
public class ChildTasksCollector extends TreeAlgorithmBase<Task>
```

收集所有子任务。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ChildTasksCollector()](#ChildTasksCollector--) | 初始化 [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | 处理指定的对象。 |
| [getTasks()](#getTasks--) | 获取收集的子对象（任务）列表。 |
### ChildTasksCollector() {#ChildTasksCollector--}
```
public ChildTasksCollector()
```


初始化 [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector) 类的新实例。

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public void alg(Task el, int level)
```


处理指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | 要处理的对象。 |
| 级别 | int | 树节点级别。 |

### getTasks() {#getTasks--}
```
public final List<Task> getTasks()
```


获取收集的子对象（任务）列表。

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - 收集的子对象（任务）列表。
