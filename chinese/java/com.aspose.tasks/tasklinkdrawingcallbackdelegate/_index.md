---
title: "TaskLinkDrawingCallbackDelegate"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示在甘特图视图中渲染任务链接时调用的回调。"
type: docs
weight: 298
url: /zh/java/com.aspose.tasks/tasklinkdrawingcallbackdelegate/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskLinkDrawingCallbackDelegate extends System.MulticastDelegate
```

表示在甘特图视图中渲染任务链接时调用的回调。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TaskLinkDrawingCallbackDelegate()](#TaskLinkDrawingCallbackDelegate--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [invoke(TaskLinkDrawingArgs args)](#invoke-com.aspose.tasks.TaskLinkDrawingArgs-) | 表示用于处理任务链接绘制事件的方法回调。 |
### TaskLinkDrawingCallbackDelegate() {#TaskLinkDrawingCallbackDelegate--}
```
public TaskLinkDrawingCallbackDelegate()
```


### invoke(TaskLinkDrawingArgs args) {#invoke-com.aspose.tasks.TaskLinkDrawingArgs-}
```
public abstract void invoke(TaskLinkDrawingArgs args)
```


表示用于处理任务链接绘制事件的方法回调。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| args | [TaskLinkDrawingArgs](../../com.aspose.tasks/tasklinkdrawingargs) | 包含回调数据的 [TaskLinkDrawingArgs](../../com.aspose.tasks/tasklinkdrawingargs) 类的实例。 |

