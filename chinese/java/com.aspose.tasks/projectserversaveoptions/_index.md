---
title: "ProjectServerSaveOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许在项目保存到 Project Server 或 Project Online 时指定其他选项。"
type: docs
weight: 227
url: /zh/java/com.aspose.tasks/projectserversaveoptions/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerSaveOptions
```

允许在项目保存到 Project Server 或 Project Online 时指定其他选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ProjectServerSaveOptions()](#ProjectServerSaveOptions--) | 初始化 [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getPollingInterval()](#getPollingInterval--) | 获取队列作业状态请求之间的间隔。 |
| [getProjectGuid()](#getProjectGuid--) | 获取项目的唯一标识符。 |
| [getProjectName()](#getProjectName--) | 获取在 Project Server \\ Project Online 项目列表中显示的项目名称。 |
| [getTimeout()](#getTimeout--) | 获取在等待 Project Server 的队列处理服务处理保存项目请求时使用的超时时间。 |
| [setPollingInterval(double value)](#setPollingInterval-double-) | 设置队列作业状态请求之间的间隔。 |
| [setProjectGuid(UUID value)](#setProjectGuid-java.util.UUID-) | 设置项目的唯一标识符。 |
| [setProjectName(String value)](#setProjectName-java.lang.String-) | 设置在 Project Server \\ Project Online 项目列表中显示的项目名称。 |
| [setTimeout(double value)](#setTimeout-double-) | 设置在等待 Project Server 的队列处理服务处理保存项目请求时使用的超时时间。 |
### ProjectServerSaveOptions() {#ProjectServerSaveOptions--}
```
public ProjectServerSaveOptions()
```


初始化 [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) 类的新实例。

### getPollingInterval() {#getPollingInterval--}
```
public final double getPollingInterval()
```


获取队列作业状态请求之间的间隔。默认值为 2 秒。

**Returns:**
double - 队列作业状态请求之间的间隔。
### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


获取项目的唯一标识符。应在 Project Server \\ Project Online 实例中唯一。

**Returns:**
java.util.UUID - 项目的唯一标识符。
### getProjectName() {#getProjectName--}
```
public final String getProjectName()
```


获取在 Project Server \\ Project Online 项目列表中显示的项目名称。应在 Project Server \\ Project Online 实例中唯一。如果省略该值，将使用 Prj.Name 属性的值。

**Returns:**
java.lang.String - 在 Project Server \\ Project Online 项目列表中显示的项目名称。
### getTimeout() {#getTimeout--}
```
public final double getTimeout()
```


获取在等待 Project Server 的队列处理服务处理保存项目请求时使用的超时时间。此属性的默认值为 1 分钟。

--------------------

对于大型项目或 Project Server 实例因响应其他请求而过于繁忙的情况，处理时间可能会更长。

**Returns:**
double - 在等待 Project Server 的队列处理服务处理保存项目请求时使用的超时时间。
### setPollingInterval(double value) {#setPollingInterval-double-}
```
public final void setPollingInterval(double value)
```


设置队列作业状态请求之间的间隔。默认值为 2 秒。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 队列作业状态请求之间的间隔。 |

### setProjectGuid(UUID value) {#setProjectGuid-java.util.UUID-}
```
public final void setProjectGuid(UUID value)
```


设置项目的唯一标识符。应在 Project Server \\ Project Online 实例中唯一。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.UUID | 项目的唯一标识符。 |

### setProjectName(String value) {#setProjectName-java.lang.String-}
```
public final void setProjectName(String value)
```


设置在 Project Server \\ Project Online 项目列表中显示的项目名称。应在 Project Server \\ Project Online 实例中唯一。如果省略该值，将使用 Prj.Name 属性的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 在 Project Server \\ Project Online 项目列表中显示的项目名称。 |

### setTimeout(double value) {#setTimeout-double-}
```
public final void setTimeout(double value)
```


设置在等待 Project Server 的队列处理服务处理保存项目请求时使用的超时时间。此属性的默认值为 1 分钟。

--------------------

对于大型项目或 Project Server 实例因响应其他请求而过于繁忙的情况，处理时间可能会更长。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 在等待 Project Server 的队列处理服务处理保存项目请求时使用的超时。 |

