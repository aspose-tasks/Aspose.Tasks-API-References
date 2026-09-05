---
title: "ExtendedAttribute"
second_title: "Aspose.Tasks for Java API Reference"
description: "확장 속성을 나타냅니다."
type: docs
weight: 81
url: /ko/java/com.aspose.tasks/extendedattribute/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttribute
```

확장 속성을 나타냅니다.

--------------------

현재 MSP Xml 2003/2007 및 mpp 2003에서 읽어오는 모든 유형의 Extended attributes를 지원합니다. MSP mpp 2007의 경우, durations와 flags를 제외한 모든 Extended attributes 읽기가 지원됩니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getAttributeDefinition()](#getAttributeDefinition--) | 속성 정의를 가져옵니다. |
| [getDateValue()](#getDateValue--) | 날짜 유형(Date, Start, Finish)을 가진 속성의 값을 가져옵니다. |
| [getDurationValue()](#getDurationValue--) | 'Duration' 유형을 가진 속성의 값을 가져옵니다. |
| [getFieldId()](#getFieldId--) | 필드의 ID를 가져옵니다. |
| [getFlagValue()](#getFlagValue--) | 'Flag' 유형을 가진 속성에 플래그가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getNumericValue()](#getNumericValue--) | 숫자 유형(Cost, Number)을 가진 속성의 값을 가져옵니다. |
| [getTextValue()](#getTextValue--) | 'Text' 유형을 가진 속성의 값을 가져옵니다. |
| [getValueGuid()](#getValueGuid--) | lookup 값의 guid를 가져옵니다. |
| [getValueReadOnly()](#getValueReadOnly--) | 이 [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) 인스턴스의 값이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. |
| [isErrorValue()](#isErrorValue--) | extended attribute 값 계산이 오류를 발생했는지 여부를 가져옵니다. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | 날짜 유형(Date, Start, Finish)을 가진 속성에 값을 설정합니다. |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | 'Duration' 유형의 속성에 대한 값을 설정합니다. |
| [setFlagValue(boolean value)](#setFlagValue-boolean-) | 'Flag' 유형의 속성에 플래그가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | 숫자 유형(비용, 숫자)의 속성에 대한 값을 설정합니다. |
| [setTextValue(String value)](#setTextValue-java.lang.String-) | 'Text' 유형의 속성에 대한 값을 설정합니다. |
| [toString()](#toString--) | 확장 속성의 짧은 문자열 표현을 반환합니다. |
### getAttributeDefinition() {#getAttributeDefinition--}
```
public final ExtendedAttributeDefinition getAttributeDefinition()
```


속성 정의를 가져옵니다.

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the attribute definition.
### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


날짜 유형(Date, Start, Finish)을 가진 속성의 값을 가져옵니다.

**Returns:**
java.util.Date - 날짜 유형(날짜, 시작, 종료)의 속성에 대한 값입니다.
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


'Duration' 유형을 가진 속성의 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - value for attributes with 'Duration' type.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


필드의 ID를 가져옵니다.

**Returns:**
java.lang.String - 필드의 ID입니다.
### getFlagValue() {#getFlagValue--}
```
public final boolean getFlagValue()
```


'Flag' 유형을 가진 속성에 플래그가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 'Flag' 유형의 속성에 플래그가 설정되었는지 여부를 나타내는 값입니다.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


숫자 유형(Cost, Number)을 가진 속성의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - 숫자 유형(비용, 숫자)의 속성에 대한 값입니다.
### getTextValue() {#getTextValue--}
```
public final String getTextValue()
```


'Text' 유형을 가진 속성의 값을 가져옵니다.

**Returns:**
java.lang.String - 'Text' 유형의 속성에 대한 값입니다.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


lookup 값의 guid를 가져옵니다.

--------------------

직접 설정해서는 안 되며, 대신 ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue)를 사용하여 조회 값이 있는 확장 속성을 생성하십시오.

**Returns:**
java.lang.String - 조회 값의 GUID입니다.
### getValueReadOnly() {#getValueReadOnly--}
```
public final boolean getValueReadOnly()
```


이 [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) 인스턴스의 값이 읽기 전용인지 여부를 나타내는 값을 가져옵니다.

Value: 이 객체에 대해 [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition)에서 수식이나 롤업이 정의된 경우 true를 반환합니다.

**Returns:**
boolean - 이 [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) 인스턴스의 값이 읽기 전용인지 여부를 나타내는 값입니다.
### isErrorValue() {#isErrorValue--}
```
public final boolean isErrorValue()
```


extended attribute 값 계산이 오류를 발생했는지 여부를 가져옵니다.

**Returns:**
boolean - 확장 속성 값 계산이 오류를 발생했는지 여부입니다.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


날짜 유형(Date, Start, Finish)을 가진 속성에 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 날짜 유형(날짜, 시작, 종료)의 속성에 대한 값입니다. |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


'Duration' 유형의 속성에 대한 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | 'Duration' 유형의 속성에 대한 값입니다. |

### setFlagValue(boolean value) {#setFlagValue-boolean-}
```
public final void setFlagValue(boolean value)
```


'Flag' 유형의 속성에 플래그가 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 'Flag' 유형의 속성에 플래그가 설정되었는지 여부를 나타내는 값입니다. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


숫자 유형(비용, 숫자)의 속성에 대한 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | 숫자 유형(비용, 숫자)의 속성에 대한 값입니다. |

### setTextValue(String value) {#setTextValue-java.lang.String-}
```
public final void setTextValue(String value)
```


'Text' 유형의 속성에 대한 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 'Text' 유형의 속성에 대한 값입니다. |

### toString() {#toString--}
```
public String toString()
```


확장 속성의 짧은 문자열 표현을 반환합니다.

**Returns:**
java.lang.String - 확장 속성의 문자열 표현입니다.
