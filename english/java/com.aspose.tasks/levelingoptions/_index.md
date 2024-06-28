---
title: LevelingOptions
second_title: Aspose.Tasks for Java API Reference
description: Allows to specify parameters of resource leveling.
type: docs
weight: 137
url: /java/com.aspose.tasks/levelingoptions/
---

**Inheritance:**
java.lang.Object
```
public final class LevelingOptions
```

Allows to specify parameters of resource leveling.
## Constructors

| Constructor | Description |
| --- | --- |
| [LevelingOptions()](#LevelingOptions--) | Initializes a new instance of the [LevelingOptions](../../com.aspose.tasks/levelingoptions) class. |
## Methods

| Method | Description |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Gets a token which can be used to cancel a project leveling operation. |
| [getFinishDate()](#getFinishDate--) | Gets leveling period end date. |
| [getLevelingOrder()](#getLevelingOrder--) | Gets the order in which the leveling algorithm delays tasks that have overallocations. |
| [getMessageHandler()](#getMessageHandler--) | Gets message handler callback which can be used to intercept log messages produced by Aspose.Tasks during resource leveling. |
| [getMessageLevel()](#getMessageLevel--) | Gets level of log messages emitted by Aspose.Tasks during resource leveling. |
| [getResources()](#getResources--) | Gets the list of the resources which will be leveled. |
| [getStartDate()](#getStartDate--) | Gets leveling period start date. |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Sets a token which can be used to cancel a project leveling operation. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Sets leveling period end date. |
| [setLevelingOrder(int value)](#setLevelingOrder-int-) | The order in which the leveling algorithm delays tasks that have overallocations. |
| [setMessageHandler(IMessageHandler value)](#setMessageHandler-com.aspose.tasks.IMessageHandler-) | Sets message handler callback which can be used to intercept log messages produced by Aspose.Tasks during resource leveling. |
| [setMessageLevel(int value)](#setMessageLevel-int-) | Sets level of log messages emitted by Aspose.Tasks during resource leveling. |
| [setResources(List&lt;Resource&gt; value)](#setResources-java.util.List-com.aspose.tasks.Resource--) | Sets the list of the resources which will be leveled. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Sets leveling period start date. |
### LevelingOptions() {#LevelingOptions--}
```
public LevelingOptions()
```


Initializes a new instance of the [LevelingOptions](../../com.aspose.tasks/levelingoptions) class.

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Gets a token which can be used to cancel a project leveling operation.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project leveling operation.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Gets leveling period end date. The default value is the project`s finish date.

**Returns:**
java.util.Date - leveling period end date.
### getLevelingOrder() {#getLevelingOrder--}
```
public final int getLevelingOrder()
```


Gets the order in which the leveling algorithm delays tasks that have overallocations. After determination of tasks causing the overallocation and which tasks can be delayed, the specified order is used which task should be delayed first.

**Returns:**
int - the order in which the leveling algorithm delays tasks that have overallocations.
### getMessageHandler() {#getMessageHandler--}
```
public final IMessageHandler getMessageHandler()
```


Gets message handler callback which can be used to intercept log messages produced by Aspose.Tasks during resource leveling.

**Returns:**
[IMessageHandler](../../com.aspose.tasks/imessagehandler) - message handler callback which can be used to intercept log messages produced by Aspose.
### getMessageLevel() {#getMessageLevel--}
```
public final int getMessageLevel()
```


Gets level of log messages emitted by Aspose.Tasks during resource leveling.

**Returns:**
int - level of log messages emitted by Aspose.
### getResources() {#getResources--}
```
public final List<Resource> getResources()
```


Gets the list of the resources which will be leveled. If null is set, all project resources will be leveled.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - the list of the resources which will be leveled.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Gets leveling period start date. The default value is the project`s start date.

**Returns:**
java.util.Date - leveling period start date.
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Sets a token which can be used to cancel a project leveling operation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | a token which can be used to cancel a project leveling operation. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


Sets leveling period end date. The default value is the project`s finish date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | leveling period end date. |

### setLevelingOrder(int value) {#setLevelingOrder-int-}
```
public final void setLevelingOrder(int value)
```


The order in which the leveling algorithm delays tasks that have overallocations. After determination of tasks causing the overallocation and which tasks can be delayed, the specified order is used which task should be delayed first.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the order in which the leveling algorithm delays tasks that have overallocations. |

### setMessageHandler(IMessageHandler value) {#setMessageHandler-com.aspose.tasks.IMessageHandler-}
```
public final void setMessageHandler(IMessageHandler value)
```


Sets message handler callback which can be used to intercept log messages produced by Aspose.Tasks during resource leveling.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IMessageHandler](../../com.aspose.tasks/imessagehandler) | message handler callback which can be used to intercept log messages produced by Aspose. |

### setMessageLevel(int value) {#setMessageLevel-int-}
```
public final void setMessageLevel(int value)
```


Sets level of log messages emitted by Aspose.Tasks during resource leveling.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | level of log messages emitted by Aspose. |

### setResources(List&lt;Resource&gt; value) {#setResources-java.util.List-com.aspose.tasks.Resource--}
```
public final void setResources(List<Resource> value)
```


Sets the list of the resources which will be leveled. If null is set, all project resources will be leveled.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Resource&gt; | the list of the resources which will be leveled. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Sets leveling period start date. The default value is the project`s start date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | leveling period start date. |

