---
title: "TaskBarTextConverter"
second_title: "Aspose.Tasks for Java API 参考"
description: "任务数据到条形文本的自定义转换器。"
type: docs
weight: 290
url: /zh/java/com.aspose.tasks/taskbartextconverter/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskBarTextConverter extends System.MulticastDelegate
```

任务数据到条形文字的自定义转换器。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TaskBarTextConverter()](#TaskBarTextConverter--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [invoke(Task task)](#invoke-com.aspose.tasks.Task-) | 任务数据到条形文字的自定义转换器。 |
### TaskBarTextConverter() {#TaskBarTextConverter--}
```
public TaskBarTextConverter()
```


### invoke(Task task) {#invoke-com.aspose.tasks.Task-}
```
public abstract String invoke(Task task)
```


任务数据到条形文字的自定义转换器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 将为其呈现任务栏文本的任务。 |

**Returns:**
java.lang.String - 对应指定任务的条形要呈现的文本。
