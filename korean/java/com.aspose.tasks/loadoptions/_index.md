---
title: "LoadOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "파일이나 스트림에서 프로젝트를 로드할 때 추가 로드 매개변수를 지정할 수 있습니다."
type: docs
weight: 148
url: /ko/java/com.aspose.tasks/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

파일이나 스트림에서 프로젝트를 로드할 때 추가 로드 매개변수를 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | 새로운 [LoadOptions](../../com.aspose/tasks/loadoptions) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | 프로젝트 로드 작업을 취소하는 데 사용할 수 있는 토큰을 가져옵니다. |
| [getEncoding()](#getEncoding--) | HTML, MPX, XER 및 Primavera XML 형식에서 프로젝트를 읽는 데 사용되는 인코딩을 가져옵니다. |
| [getErrorHandler()](#getErrorHandler--) | XML 구문 분석 오류를 처리하기 위한 콜백 메서드를 가져옵니다. |
| [getPassword()](#getPassword--) | 보호 비밀번호를 가져옵니다. |
| [getPrimaveraReadOptions()](#getPrimaveraReadOptions--) | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 클래스의 지정된 인스턴스를 가져옵니다. 이 인스턴스는 Primavera 형식(Primavera P6 XER 또는 Primavera P6 Xml) 로드 동작을 사용자 지정하는 데 사용할 수 있습니다. |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | 프로젝트 로드 작업을 취소하는 데 사용할 수 있는 토큰을 설정합니다. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | HTML, MPX, XER 및 Primavera XML 형식에서 프로젝트를 읽는 데 사용되는 인코딩을 설정합니다. |
| [setErrorHandler(ParseErrorCallback value)](#setErrorHandler-com.aspose.tasks.ParseErrorCallback-) | XML 구문 분석 오류를 처리하기 위한 콜백 메서드를 설정합니다. |
| [setPassword(String value)](#setPassword-java.lang.String-) | 보호 비밀번호를 설정합니다. |
| [setPrimaveraReadOptions(PrimaveraReadOptions value)](#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-) | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 클래스의 지정된 인스턴스를 설정합니다. 이 인스턴스는 Primavera 형식(Primavera P6 XER 또는 Primavera P6 Xml) 로드 동작을 사용자 지정하는 데 사용할 수 있습니다. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


새로운 [LoadOptions](../../com.aspose/tasks/loadoptions) 클래스 인스턴스를 초기화합니다.

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


프로젝트 로드 작업을 취소하는 데 사용할 수 있는 토큰을 가져옵니다.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project loading operation.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


HTML, MPX, XER 및 Primavera XML 형식에서 프로젝트를 읽는 데 사용되는 인코딩을 가져옵니다. 기본 인코딩은 UTF8입니다.

**Returns:**
java.nio.charset.Charset - HTML, MPX, XER 및 Primavera XML 형식에서 프로젝트를 읽는 데 사용되는 인코딩.
### getErrorHandler() {#getErrorHandler--}
```
public final ParseErrorCallback getErrorHandler()
```


XML 구문 분석 오류를 처리하기 위한 콜백 메서드를 가져옵니다.

**Returns:**
[ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) - a callback method to handle xml parse errors.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


보호 비밀번호를 가져옵니다.

**Returns:**
java.lang.String - 보호 비밀번호.
### getPrimaveraReadOptions() {#getPrimaveraReadOptions--}
```
public final PrimaveraReadOptions getPrimaveraReadOptions()
```


[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 클래스의 지정된 인스턴스를 가져옵니다. 이 인스턴스는 Primavera 형식(Primavera P6 XER 또는 Primavera P6 Xml) 로드 동작을 사용자 지정하는 데 사용할 수 있습니다.

**Returns:**
[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) - a specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class which can be used to customize the behavior of loading Primavera formats (Primavera P6 XER or Primavera P6 Xml).
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


프로젝트 로드 작업을 취소하는 데 사용할 수 있는 토큰을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | 프로젝트 로드 작업을 취소하는 데 사용할 수 있는 토큰. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


HTML, MPX, XER 및 Primavera XML 형식에서 프로젝트를 읽는 데 사용되는 인코딩을 설정합니다. 기본 인코딩은 UTF8입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.nio.charset.Charset | HTML, MPX, XER 및 Primavera XML 형식에서 프로젝트를 읽는 데 사용되는 인코딩. |

### setErrorHandler(ParseErrorCallback value) {#setErrorHandler-com.aspose.tasks.ParseErrorCallback-}
```
public final void setErrorHandler(ParseErrorCallback value)
```


XML 구문 분석 오류를 처리하기 위한 콜백 메서드를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | XML 구문 분석 오류를 처리하기 위한 콜백 메서드. |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


보호 비밀번호를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 보호 비밀번호. |

### setPrimaveraReadOptions(PrimaveraReadOptions value) {#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-}
```
public final void setPrimaveraReadOptions(PrimaveraReadOptions value)
```


[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 클래스의 지정된 인스턴스를 설정합니다. 이 인스턴스는 Primavera 형식(Primavera P6 XER 또는 Primavera P6 Xml) 로드 동작을 사용자 지정하는 데 사용할 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 클래스의 지정된 인스턴스로, Primavera 형식(Primavera P6 XER 또는 Primavera P6 Xml) 로드 동작을 사용자 지정하는 데 사용할 수 있습니다. |

