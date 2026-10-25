---
title: "VbaModule"
second_title: "Aspose.Tasks for Java API Reference"
description: "VBA 모듈을 나타냅니다."
type: docs
weight: 334
url: /ko/java/com.aspose.tasks/vbamodule/
---

**Inheritance:**
java.lang.Object
```
public final class VbaModule
```

VBA 모듈을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [createClassModule(String name)](#createClassModule-java.lang.String-) | [VbaModule](../../com.aspose/tasks/vbamodule)의 VbaModuleType.ClassModule 유형 인스턴스를 생성합니다. |
| [createProceduralModule(String name)](#createProceduralModule-java.lang.String-) | VbaModuleType.ProceduralModule 유형으로 [VbaModule](../../com.aspose.tasks/vbamodule)의 인스턴스를 생성합니다. |
| [getAttributes()](#getAttributes--) | 모듈의 속성 컬렉션을 가져옵니다. |
| [getName()](#getName--) | VBA 모듈의 이름을 가져옵니다. |
| [getSourceCode()](#getSourceCode--) | VBA 모듈의 소스 코드를 가져옵니다. |
| [getType()](#getType--) | 모듈의 유형을 가져옵니다. |
| [setName(String value)](#setName-java.lang.String-) | VBA 모듈의 이름 |
| [setSourceCode(String value)](#setSourceCode-java.lang.String-) | VBA 모듈의 소스 코드를 설정합니다. |
### createClassModule(String name) {#createClassModule-java.lang.String-}
```
public static VbaModule createClassModule(String name)
```


[VbaModule](../../com.aspose/tasks/vbamodule)의 VbaModuleType.ClassModule 유형 인스턴스를 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### createProceduralModule(String name) {#createProceduralModule-java.lang.String-}
```
public static VbaModule createProceduralModule(String name)
```


VbaModuleType.ProceduralModule 유형으로 [VbaModule](../../com.aspose.tasks/vbamodule)의 인스턴스를 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### getAttributes() {#getAttributes--}
```
public final VbaModuleAttributeCollection getAttributes()
```


모듈의 속성 컬렉션을 가져옵니다.

**Returns:**
[VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection) - a collection of the module's attributes.
### getName() {#getName--}
```
public final String getName()
```


VBA 모듈의 이름을 가져옵니다.

**Returns:**
java.lang.String - VBA 모듈의 이름
### getSourceCode() {#getSourceCode--}
```
public final String getSourceCode()
```


VBA 모듈의 소스 코드를 가져옵니다.

**Returns:**
java.lang.String - VBA 모듈의 소스 코드
### getType() {#getType--}
```
public final int getType()
```


모듈의 유형을 가져옵니다.

**Returns:**
int - 모듈의 유형.
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


VBA 모듈의 이름

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | VBA 모듈의 이름 |

### setSourceCode(String value) {#setSourceCode-java.lang.String-}
```
public final void setSourceCode(String value)
```


VBA 모듈의 소스 코드를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | VBA 모듈의 소스 코드 |

