---
title: "LevelingOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许指定资源平衡的参数。"
type: docs
weight: 142
url: /zh/java/com.aspose.tasks/levelingoptions/
---

**Inheritance:**
java.lang.Object
```
public final class LevelingOptions
```

允许指定资源平衡的参数。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LevelingOptions()](#LevelingOptions--) | 初始化一个新的 [LevelingOptions](../../com.aspose.tasks/levelingoptions) 类的实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | 获取可用于取消项目平衡操作的令牌。 |
| [getFinishDate()](#getFinishDate--) | 获取平衡期间结束日期。 |
| [getLevelingOrder()](#getLevelingOrder--) | 获取平衡算法延迟具有超额分配任务的顺序。 |
| [getMessageHandler()](#getMessageHandler--) | 获取可用于拦截 Aspose.Tasks 在资源平衡期间产生的日志消息的消息处理程序回调。 |
| [getMessageLevel()](#getMessageLevel--) | 获取 Aspose.Tasks 在资源平衡期间发出的日志消息级别。 |
| [getResources()](#getResources--) | 获取将被平衡的资源列表。 |
| [getStartDate()](#getStartDate--) | 获取平衡期间开始日期。 |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | 设置可用于取消项目平衡操作的令牌。 |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | 设置平衡期间结束日期。 |
| [setLevelingOrder(int value)](#setLevelingOrder-int-) | 平衡算法延迟具有超额分配任务的顺序。 |
| [setMessageHandler(IMessageHandler value)](#setMessageHandler-com.aspose.tasks.IMessageHandler-) | 设置可用于拦截 Aspose.Tasks 在资源平衡期间产生的日志消息的消息处理程序回调。 |
| [setMessageLevel(int value)](#setMessageLevel-int-) | 设置 Aspose.Tasks 在资源平衡期间发出的日志消息级别。 |
| [setResources(List&lt;Resource&gt; value)](#setResources-java.util.List-com.aspose.tasks.Resource--) | 设置将被平衡的资源列表。 |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | 设置平衡期间开始日期。 |
### LevelingOptions() {#LevelingOptions--}
```
public LevelingOptions()
```


初始化一个新的 [LevelingOptions](../../com.aspose.tasks/levelingoptions) 类的实例。

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


获取可用于取消项目平衡操作的令牌。

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project leveling operation.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


获取平衡期间结束日期。默认值为 project`s 的完成日期。

**Returns:**
java.util.Date - 平衡期间结束日期。
### getLevelingOrder() {#getLevelingOrder--}
```
public final int getLevelingOrder()
```


获取平衡算法延迟具有超额分配的任务的顺序。在确定导致超额分配的任务以及哪些任务可以被延迟后，使用指定的顺序来决定首先应延迟哪个任务。

**Returns:**
int - 平衡算法延迟具有超额分配的任务的顺序。
### getMessageHandler() {#getMessageHandler--}
```
public final IMessageHandler getMessageHandler()
```


获取可用于拦截 Aspose.Tasks 在资源平衡期间产生的日志消息的消息处理程序回调。

**Returns:**
[IMessageHandler](../../com.aspose.tasks/imessagehandler) - message handler callback which can be used to intercept log messages produced by Aspose.
### getMessageLevel() {#getMessageLevel--}
```
public final int getMessageLevel()
```


获取 Aspose.Tasks 在资源平衡期间发出的日志消息级别。

**Returns:**
int - Aspose 发出的日志消息级别。
### getResources() {#getResources--}
```
public final List<Resource> getResources()
```


获取将被平衡的资源列表。如果设置为 null，则所有项目资源都将被平衡。

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - 将被平衡的资源列表。
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


获取平衡期间开始日期。默认值为 project`s 的开始日期。

**Returns:**
java.util.Date - 平衡期间开始日期。
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


设置可用于取消项目平衡操作的令牌。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | 可用于取消项目平衡操作的令牌。 |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


设置平衡期间结束日期。默认值为 project`s 的完成日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 平衡期间结束日期。 |

### setLevelingOrder(int value) {#setLevelingOrder-int-}
```
public final void setLevelingOrder(int value)
```


平衡算法延迟具有超额分配的任务的顺序。在确定导致超额分配的任务以及哪些任务可以被延迟后，使用指定的顺序来决定首先应延迟哪个任务。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 平衡算法延迟具有超额分配的任务的顺序。 |

### setMessageHandler(IMessageHandler value) {#setMessageHandler-com.aspose.tasks.IMessageHandler-}
```
public final void setMessageHandler(IMessageHandler value)
```


设置可用于拦截 Aspose.Tasks 在资源平衡期间产生的日志消息的消息处理程序回调。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IMessageHandler](../../com.aspose.tasks/imessagehandler) | 可用于拦截 Aspose 生成的日志消息的消息处理程序回调。 |

### setMessageLevel(int value) {#setMessageLevel-int-}
```
public final void setMessageLevel(int value)
```


设置 Aspose.Tasks 在资源平衡期间发出的日志消息级别。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | Aspose 发出的日志消息级别。 |

### setResources(List&lt;Resource&gt; value) {#setResources-java.util.List-com.aspose.tasks.Resource--}
```
public final void setResources(List<Resource> value)
```


设置将被平衡的资源列表。如果设置为 null，则所有项目资源都将被平衡。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.List&lt;com.aspose.tasks.Resource&gt; | 将被平衡的资源列表。 |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


设置平衡期间开始日期。默认值为 project`s 的开始日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 平衡期间开始日期。 |

