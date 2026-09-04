---
title: "LoadOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许在从文件或流加载项目时指定其他加载参数。"
type: docs
weight: 148
url: /zh/java/com.aspose.tasks/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

允许在从文件或流加载项目时指定其他加载参数。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | 初始化 [LoadOptions](../../com.aspose/tasks/loadoptions) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | 获取可用于取消项目加载操作的令牌。 |
| [getEncoding()](#getEncoding--) | 获取用于从 HTML、MPX、XER 和 Primavera XML 格式读取项目的编码。 |
| [getErrorHandler()](#getErrorHandler--) | 获取用于处理 XML 解析错误的回调方法。 |
| [getPassword()](#getPassword--) | 获取保护密码。 |
| [getPrimaveraReadOptions()](#getPrimaveraReadOptions--) | 获取 [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 类的指定实例，可用于自定义加载 Primavera 格式（Primavera P6 XER 或 Primavera P6 Xml）的行为。 |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | 设置可用于取消项目加载操作的令牌。 |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | 设置用于从 HTML、MPX、XER 和 Primavera XML 格式读取项目的编码。 |
| [setErrorHandler(ParseErrorCallback value)](#setErrorHandler-com.aspose.tasks.ParseErrorCallback-) | 设置用于处理 XML 解析错误的回调方法。 |
| [setPassword(String value)](#setPassword-java.lang.String-) | 设置保护密码。 |
| [setPrimaveraReadOptions(PrimaveraReadOptions value)](#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-) | 设置 [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 类的指定实例，可用于自定义加载 Primavera 格式（Primavera P6 XER 或 Primavera P6 Xml）的行为。 |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


初始化 [LoadOptions](../../com.aspose/tasks/loadoptions) 类的新实例。

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


获取可用于取消项目加载操作的令牌。

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project loading operation.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


获取用于从 HTML、MPX、XER 和 Primavera XML 格式读取项目的编码。默认编码为 UTF8。

**Returns:**
java.nio.charset.Charset - 用于从 HTML、MPX、XER 和 Primavera XML 格式读取项目的编码。
### getErrorHandler() {#getErrorHandler--}
```
public final ParseErrorCallback getErrorHandler()
```


获取用于处理 XML 解析错误的回调方法。

**Returns:**
[ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) - a callback method to handle xml parse errors.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


获取保护密码。

**Returns:**
java.lang.String - 一个保护密码。
### getPrimaveraReadOptions() {#getPrimaveraReadOptions--}
```
public final PrimaveraReadOptions getPrimaveraReadOptions()
```


获取 [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 类的指定实例，可用于自定义加载 Primavera 格式（Primavera P6 XER 或 Primavera P6 Xml）的行为。

**Returns:**
[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) - a specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class which can be used to customize the behavior of loading Primavera formats (Primavera P6 XER or Primavera P6 Xml).
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


设置可用于取消项目加载操作的令牌。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | 一个可用于取消项目加载操作的令牌。 |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


设置用于从 HTML、MPX、XER 和 Primavera XML 格式读取项目的编码。默认编码为 UTF8。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.nio.charset.Charset | 用于从 HTML、MPX、XER 和 Primavera XML 格式读取项目的编码。 |

### setErrorHandler(ParseErrorCallback value) {#setErrorHandler-com.aspose.tasks.ParseErrorCallback-}
```
public final void setErrorHandler(ParseErrorCallback value)
```


设置用于处理 XML 解析错误的回调方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | 用于处理 XML 解析错误的回调方法。 |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


设置保护密码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 一个保护密码。 |

### setPrimaveraReadOptions(PrimaveraReadOptions value) {#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-}
```
public final void setPrimaveraReadOptions(PrimaveraReadOptions value)
```


设置 [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 类的指定实例，可用于自定义加载 Primavera 格式（Primavera P6 XER 或 Primavera P6 Xml）的行为。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | 一个 [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 类的指定实例，可用于自定义加载 Primavera 格式（Primavera P6 XER 或 Primavera P6 Xml）的行为。 |

