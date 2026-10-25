---
title: "SimpleSaveOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "这是一个抽象基类，允许用户在将项目保存为特定格式时指定基本选项。"
type: docs
weight: 277
url: /zh/java/com.aspose.tasks/simplesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SimpleSaveOptions
```

这是一个抽象基类，允许用户在将项目保存为特定格式时指定基本选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SimpleSaveOptions()](#SimpleSaveOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--) | 获取如果使用此保存选项对象，文档将被保存的格式。 |
| [getTasksComparer()](#getTasksComparer--) | 获取用于在甘特图和任务表图上排序任务的比较器。 |
| [getTasksFilter()](#getTasksFilter--) | 获取用于过滤在甘特图、任务表和任务使用图上呈现的任务的条件。 |
| [setTasksComparer(Comparator&lt;Task&gt; value)](#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--) | 设置用于在甘特图和任务表图上排序任务的比较器。 |
| [setTasksFilter(ICondition&lt;Task&gt; value)](#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | 设置用于过滤在甘特图、任务表和任务使用图上呈现的任务的条件。 |
### SimpleSaveOptions() {#SimpleSaveOptions--}
```
public SimpleSaveOptions()
```


### getSaveFormat() {#getSaveFormat--}
```
public final int getSaveFormat()
```


获取如果使用此保存选项对象，文档将被保存的格式。

**Returns:**
int - 文档将被保存的 [SaveFileFormat](../../com.aspose.tasks/savefileformat) 。
### getTasksComparer() {#getTasksComparer--}
```
public final Comparator<Task> getTasksComparer()
```


获取用于在甘特图和任务表图上排序任务的比较器。

**Returns:**
java.util.Comparator&lt;com.aspose.tasks.Task&gt; - 用于在甘特图和任务表图上排序任务的比较器。
### getTasksFilter() {#getTasksFilter--}
```
public final ICondition<Task> getTasksFilter()
```


获取用于过滤在甘特图、任务表和任务使用图上呈现的任务的条件。

--------------------

如果未指定值，则使用默认过滤器，该过滤器会移除不可见的任务——即折叠任务的子任务。

**Returns:**
[ICondition](../../com.aspose.tasks/icondition) - the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.
### setTasksComparer(Comparator&lt;Task&gt; value) {#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--}
```
public final void setTasksComparer(Comparator<Task> value)
```


设置用于在甘特图和任务表图上排序任务的比较器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Comparator&lt;com.aspose.tasks.Task&gt; | 用于在甘特图和任务表图上排序任务的比较器。 |

### setTasksFilter(ICondition&lt;Task&gt; value) {#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public final void setTasksFilter(ICondition<Task> value)
```


设置用于过滤在甘特图、任务表和任务使用图上呈现的任务的条件。

--------------------

如果未指定值，则使用默认过滤器，该过滤器会移除不可见的任务——即折叠任务的子任务。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | 用于过滤在甘特图、任务表和任务使用图上呈现的任务的条件。 |

