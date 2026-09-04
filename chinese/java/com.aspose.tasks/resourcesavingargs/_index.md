---
title: "ResourceSavingArgs"
second_title: "Aspose.Tasks for Java API 参考"
description: "此类表示一组与在转换为 HTML 格式期间发生的外部资源文件保存相关的数据。"
type: docs
weight: 254
url: /zh/java/com.aspose.tasks/resourcesavingargs/
---

**Inheritance:**
java.lang.Object
```
public class ResourceSavingArgs
```

此类表示与在转换为 HTML 格式期间发生的外部资源文件保存相关的数据集。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ResourceSavingArgs()](#ResourceSavingArgs--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [closeStreamIfRequired()](#closeStreamIfRequired--) | 如果 KeepStreamOpen 为 false，则关闭流；否则刷新流。 |
| [getFileName()](#getFileName--) | 获取从转换器传递到自定义方法代码的预期文件名。 |
| [getKeepStreamOpen()](#getKeepStreamOpen--) | 获取一个值，指示资源保存完成后流是否保持打开。 |
| [getStream()](#getStream--) | 获取已保存文件的二进制内容。 |
| [getUri()](#getUri--) | 获取资源 URI。 |
| [setFileName(String value)](#setFileName-java.lang.String-) | 设置从转换器传递到自定义方法代码的假定文件名。 |
| [setKeepStreamOpen(boolean value)](#setKeepStreamOpen-boolean-) | 设置一个值，指示在资源保存完成后流是否保持打开。 |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | 设置已保存文件的二进制内容。 |
| [setUri(String value)](#setUri-java.lang.String-) | 设置资源 URI。 |
### ResourceSavingArgs() {#ResourceSavingArgs--}
```
public ResourceSavingArgs()
```


### closeStreamIfRequired() {#closeStreamIfRequired--}
```
public final void closeStreamIfRequired()
```


如果 KeepStreamOpen 为 false，则关闭流；否则刷新流。

### getFileName() {#getFileName--}
```
public final String getFileName()
```


获取从转换器传递到自定义方法代码的假定文件名。可在自定义代码中用于决定如何处理或将文件保存到何处。

**Returns:**
java.lang.String - 从转换器传递到自定义方法代码的假定文件名。
### getKeepStreamOpen() {#getKeepStreamOpen--}
```
public final boolean getKeepStreamOpen()
```


获取一个值，指示资源保存完成后流是否保持打开。

**Returns:**
boolean - 一个指示在资源保存完成后流是否保持打开的值。
### getStream() {#getStream--}
```
public final OutputStream getStream()
```


获取已保存文件的二进制内容。

**Returns:**
java.io.OutputStream - 已保存文件的二进制内容。
### getUri() {#getUri--}
```
public final String getUri()
```


获取资源 URI。

**Returns:**
java.lang.String - 资源 URI。
### setFileName(String value) {#setFileName-java.lang.String-}
```
public final void setFileName(String value)
```


设置从转换器传递到自定义方法代码的假定文件名。可在自定义代码中用于决定如何处理或将文件保存到何处。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 从转换器传递到自定义方法代码的假定文件名。 |

### setKeepStreamOpen(boolean value) {#setKeepStreamOpen-boolean-}
```
public final void setKeepStreamOpen(boolean value)
```


设置一个值，指示在资源保存完成后流是否保持打开。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示在资源保存完成后流是否保持打开的值。 |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public final void setStream(OutputStream value)
```


设置已保存文件的二进制内容。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.io.OutputStream | 已保存文件的二进制内容。 |

### setUri(String value) {#setUri-java.lang.String-}
```
public final void setUri(String value)
```


设置资源 URI。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 资源 URI。 |

