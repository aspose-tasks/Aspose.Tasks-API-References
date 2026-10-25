---
title: "ResourceSavingArgs"
second_title: "Aspose.Tasks for Java API Reference"
description: "이 클래스는 HTML 형식으로 변환하는 동안 발생하는 외부 리소스 파일 저장과 관련된 데이터 집합을 나타냅니다."
type: docs
weight: 254
url: /ko/java/com.aspose.tasks/resourcesavingargs/
---

**Inheritance:**
java.lang.Object
```
public class ResourceSavingArgs
```

이 클래스는 HTML 형식으로 변환되는 동안 발생하는 외부 리소스 파일 저장과 관련된 데이터 집합을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ResourceSavingArgs()](#ResourceSavingArgs--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [closeStreamIfRequired()](#closeStreamIfRequired--) | KeepStreamOpen이 false이면 스트림을 닫고, 그렇지 않으면 플러시합니다. |
| [getFileName()](#getFileName--) | 변환기에서 사용자 지정 메서드 코드로 전달되는 예상 파일 이름을 가져옵니다. |
| [getKeepStreamOpen()](#getKeepStreamOpen--) | 리소스 저장이 완료된 후 스트림을 열어 둘지 여부를 나타내는 값을 가져옵니다. |
| [getStream()](#getStream--) | 저장된 파일의 바이너리 내용을 가져옵니다. |
| [getUri()](#getUri--) | 리소스 URI를 가져옵니다. |
| [setFileName(String value)](#setFileName-java.lang.String-) | 컨버터에서 사용자 정의 메서드 코드로 전달되는 가정된 파일 이름을 설정합니다. |
| [setKeepStreamOpen(boolean value)](#setKeepStreamOpen-boolean-) | 리소스 저장이 완료된 후 스트림을 계속 열어둘지 여부를 나타내는 값을 설정합니다. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | 저장된 파일의 바이너리 내용을 설정합니다. |
| [setUri(String value)](#setUri-java.lang.String-) | 리소스 URI를 설정합니다. |
### ResourceSavingArgs() {#ResourceSavingArgs--}
```
public ResourceSavingArgs()
```


### closeStreamIfRequired() {#closeStreamIfRequired--}
```
public final void closeStreamIfRequired()
```


KeepStreamOpen이 false이면 스트림을 닫고, 그렇지 않으면 플러시합니다.

### getFileName() {#getFileName--}
```
public final String getFileName()
```


컨버터에서 사용자 정의 메서드 코드로 전달되는 가정된 파일 이름을 가져옵니다. 이 파일 이름은 사용자 정의 코드에서 처리 방법이나 저장 위치를 결정하는 데 사용할 수 있습니다.

**Returns:**
java.lang.String - 컨버터에서 사용자 정의 메서드 코드로 전달되는 가정된 파일 이름.
### getKeepStreamOpen() {#getKeepStreamOpen--}
```
public final boolean getKeepStreamOpen()
```


리소스 저장이 완료된 후 스트림을 열어 둘지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 리소스 저장이 완료된 후 스트림을 계속 열어둘지 여부를 나타내는 값.
### getStream() {#getStream--}
```
public final OutputStream getStream()
```


저장된 파일의 바이너리 내용을 가져옵니다.

**Returns:**
java.io.OutputStream - 저장된 파일의 바이너리 내용.
### getUri() {#getUri--}
```
public final String getUri()
```


리소스 URI를 가져옵니다.

**Returns:**
java.lang.String - 리소스 URI.
### setFileName(String value) {#setFileName-java.lang.String-}
```
public final void setFileName(String value)
```


컨버터에서 사용자 정의 메서드 코드로 전달되는 가정된 파일 이름을 설정합니다. 이 파일 이름은 사용자 정의 코드에서 처리 방법이나 저장 위치를 결정하는 데 사용할 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 컨버터에서 사용자 정의 메서드 코드로 전달되는 가정된 파일 이름. |

### setKeepStreamOpen(boolean value) {#setKeepStreamOpen-boolean-}
```
public final void setKeepStreamOpen(boolean value)
```


리소스 저장이 완료된 후 스트림을 계속 열어둘지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 리소스 저장이 완료된 후 스트림을 계속 열어둘지 여부를 나타내는 값. |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public final void setStream(OutputStream value)
```


저장된 파일의 바이너리 내용을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.io.OutputStream | 저장된 파일의 바이너리 내용. |

### setUri(String value) {#setUri-java.lang.String-}
```
public final void setUri(String value)
```


리소스 URI를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 리소스 URI. |

