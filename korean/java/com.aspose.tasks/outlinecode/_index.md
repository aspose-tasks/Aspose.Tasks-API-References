---
title: "OutlineCode"
second_title: "Aspose.Tasks for Java API Reference"
description: "개요 코드의 값을 나타냅니다."
type: docs
weight: 167
url: /ko/java/com.aspose.tasks/outlinecode/
---

**Inheritance:**
java.lang.Object
```
public class OutlineCode
```

개요 코드의 값을 나타냅니다.

--------------------

두 개의 데이터가 필요합니다 - FieldId로 지정된 개요 코드 테이블에 대한 포인터와 ValueId 또는 ValueGuid 포인터로 지정된 값 목록에 대한 값.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [OutlineCode()](#OutlineCode--) | [OutlineCode](../../com.aspose.tasks/outlinecode) 클래스의 새 인스턴스를 초기화합니다. |
| [OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)](#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-) | 지정된 Outline Code와 그 값 중 하나를 사용하여 [OutlineCode](../../com.aspose.tasks/outlinecode) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getFieldId()](#getFieldId--) | 프로젝트 Id 사용자 정의 필드의 숫자 값을 가져옵니다. |
| [getValueGuid()](#getValueGuid--) | 값 목록에 있는 값의 GUID를 가져옵니다. |
| [getValueId()](#getValueId--) | 개요 코드 컬렉션의 정의와 연결된 값 목록의 Id를 가져옵니다. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | 프로젝트 Id 사용자 정의 필드의 숫자 값을 설정합니다. |
| [setValueGuid(String value)](#setValueGuid-java.lang.String-) | 값 목록에 있는 값의 GUID를 설정합니다. |
| [setValueId(int value)](#setValueId-int-) | 개요 코드 컬렉션의 정의와 연결된 값 목록의 Id를 설정합니다. |
### OutlineCode() {#OutlineCode--}
```
public OutlineCode()
```


[OutlineCode](../../com.aspose.tasks/outlinecode) 클래스의 새 인스턴스를 초기화합니다.

### OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue) {#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-}
```
public OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)
```


지정된 Outline Code와 그 값 중 하나를 사용하여 [OutlineCode](../../com.aspose.tasks/outlinecode) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| codeDefinition | [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition) | 개요 코드 정의. |
| outlineValue | [OutlineValue](../../com.aspose.tasks/outlinevalue) | 개요 코드 정의 값 중 하나. |

### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


프로젝트 Id 사용자 정의 필드의 숫자 값을 가져옵니다.

**Returns:**
java.lang.String - 프로젝트 Id 사용자 정의 필드의 숫자 값.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


값 목록에 있는 값의 GUID를 가져옵니다. ValueGuid는 값 목록의 FieldGuid와 일치합니다.

**Returns:**
java.lang.String - 값 목록에 있는 값의 GUID.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


개요 코드 컬렉션의 정의와 연결된 값 목록의 Id를 가져옵니다.

**Returns:**
int - 개요 코드 컬렉션의 정의와 연결된 값 목록의 Id.
### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


프로젝트 Id 사용자 정의 필드의 숫자 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 프로젝트 Id 사용자 정의 필드의 숫자 값. |

### setValueGuid(String value) {#setValueGuid-java.lang.String-}
```
public final void setValueGuid(String value)
```


값 목록에 있는 값의 GUID를 설정합니다. ValueGuid는 값 목록의 FieldGuid와 일치합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 값 목록에 있는 값의 GUID. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


개요 코드 컬렉션의 정의와 연결된 값 목록의 Id를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 개요 코드 컬렉션에 있는 정의와 연결된 값 목록의 Id. |

