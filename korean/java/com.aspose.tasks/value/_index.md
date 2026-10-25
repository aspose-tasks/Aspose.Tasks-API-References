---
title: "값"
second_title: "Aspose.Tasks for Java API Reference"
description: "값 목록의 값을 나타냅니다."
type: docs
weight: 333
url: /ko/java/com.aspose.tasks/value/
---

**Inheritance:**
java.lang.Object
```
public class Value
```

값 목록의 값을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Value()](#Value--) | 새 인스턴스를 초기화합니다 [Value](../../com.aspose/tasks/value) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getDateValue()](#getDateValue--) | DateTime으로 표현될 수 있는 경우 실제 값을 가져옵니다. |
| [getDescription()](#getDescription--) | 값의 설명을 가져옵니다. |
| [getDuration()](#getDuration--) | Duration을 나타내는 데 사용되는 실제 값을 가져옵니다. |
| [getId()](#getId--) | 프로젝트 전체에서 값의 고유 식별자를 가져옵니다. |
| [getNumericValue()](#getNumericValue--) | 숫자 또는 비용 값을 나타내는 데 사용되는 실제 값을 가져옵니다. |
| [getPhonetic()](#getPhonetic--) | 사용자 정의 필드 이름에 대한 음성 정보를 가져옵니다. |
| [getStringValue()](#getStringValue--) | 텍스트 문자열을 나타내는 데 사용되는 실제 값을 가져옵니다. |
| [getVal()](#getVal--) | 내부 표현에서 실제 값을 가져옵니다. |
| [getValueGuid()](#getValueGuid--) | 전체 프로젝트에서 이 값을 다른 값과 구별하는 GUID를 가져옵니다. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | DateTime으로 표현될 수 있는 경우 실제 값을 설정합니다. |
| [setDescription(String value)](#setDescription-java.lang.String-) | 값의 설명을 설정합니다. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Duration을 나타내는 데 사용되는 실제 값을 설정합니다. |
| [setId(int value)](#setId-int-) | 프로젝트 전체에서 값의 고유 식별자를 설정합니다. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | 숫자 또는 비용 값을 나타내는 데 사용되는 실제 값을 설정합니다. |
| [setPhonetic(String value)](#setPhonetic-java.lang.String-) | 사용자 정의 필드 이름에 대한 음성 정보를 설정합니다. |
| [setStringValue(String value)](#setStringValue-java.lang.String-) | 텍스트 문자열을 나타내는 데 사용되는 실제 값을 설정합니다. |
| [setVal(String value)](#setVal-java.lang.String-) | 내부 표현에서 실제 값을 설정합니다. |
### Value() {#Value--}
```
public Value()
```


새 인스턴스를 초기화합니다 [Value](../../com.aspose/tasks/value) 클래스.

### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


DateTime으로 표현될 수 있는 경우 실제 값을 가져옵니다. 기본값은 DateTime\#MinValue.MinValue입니다.

--------------------

DateTime 값을 설정해야 할 때, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))보다 이 속성을 사용하는 것이 좋습니다.

**Returns:**
java.util.Date - DateTime으로 표현될 수 있는 실제 값입니다.
### getDescription() {#getDescription--}
```
public final String getDescription()
```


값의 설명을 가져옵니다.

**Returns:**
java.lang.String - 값에 대한 설명입니다.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Duration을 나타내는 데 사용되는 실제 값을 가져옵니다.

--------------------

Duration 값을 설정해야 할 때, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))보다 이 속성을 사용하는 것이 좋습니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the actual value which is used to represent Duration.
### getId() {#getId--}
```
public final int getId()
```


프로젝트 전체에서 값의 고유 식별자를 가져옵니다.

다른 [Value](../../com.aspose.tasks/value) 인스턴스에 대해 동일한 식별자를 사용하지 않는 것이 중요합니다.

최소 `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) 값은 `1`입니다.

**Returns:**
int - 프로젝트 전체에서 값의 고유 식별자입니다.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


숫자 또는 비용 값을 나타내는 데 사용되는 실제 값을 가져옵니다.

--------------------

Number 또는 Cost 값을 설정해야 할 때, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))보다 이 속성을 사용하는 것이 좋습니다.

**Returns:**
java.math.BigDecimal - 숫자 또는 비용 값을 나타내는 실제 값입니다.
### getPhonetic() {#getPhonetic--}
```
public final String getPhonetic()
```


사용자 정의 필드 이름에 대한 음성 정보를 가져옵니다.

**Returns:**
java.lang.String - 사용자 정의 필드 이름에 대한 발음 정보입니다.
### getStringValue() {#getStringValue--}
```
public final String getStringValue()
```


텍스트 문자열을 나타내는 데 사용되는 실제 값을 가져옵니다.

--------------------

Text 값을 설정해야 할 때, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))보다 이 속성을 사용하는 것이 좋습니다.

**Returns:**
java.lang.String - Text 문자열을 나타내는 실제 값입니다.
### getVal() {#getVal--}
```
public final String getVal()
```


내부 표현에서 실제 값을 가져옵니다. 아래에 나열된 강력히 형식화된 속성을 사용하는 것이 좋습니다.

--------------------

Text 값을 설정하려면 강력히 형식화된 `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)) 속성을 사용하는 것이 좋습니다.

Number 또는 Cost 값을 설정하려면 강력히 형식화된 `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)) 속성을 사용하는 것이 좋습니다.

Date/Start/Finish 값을 설정하려면 강력히 형식화된 `DateValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) 속성을 사용하는 것이 좋습니다.

Duration 값을 설정하려면 강력히 형식화된 `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)) 속성을 사용하는 것이 좋습니다.

목록에 없는 유형인 경우, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) 속성을 사용하십시오.

**Returns:**
java.lang.String - 내부 표현에서의 실제 값입니다.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


전체 프로젝트에서 이 값을 다른 값과 구별하는 GUID를 가져옵니다.

**Returns:**
java.util.UUID - 전체 프로젝트에서 이 값을 다른 값들과 구분하는 GUID입니다.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


DateTime으로 표현될 수 있는 경우 실제 값을 설정합니다. 기본값은 DateTime\#MinValue.MinValue입니다.

--------------------

DateTime 값을 설정해야 할 때, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))보다 이 속성을 사용하는 것이 좋습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | DateTime으로 표현될 수 있는 실제 값입니다. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


값의 설명을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 값에 대한 설명입니다. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Duration을 나타내는 데 사용되는 실제 값을 설정합니다.

--------------------

Duration 값을 설정해야 할 때, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))보다 이 속성을 사용하는 것이 좋습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Duration을 나타내는 실제 값입니다. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


프로젝트 전체에서 값의 고유 식별자를 설정합니다.

다른 [Value](../../com.aspose.tasks/value) 인스턴스에 대해 동일한 식별자를 사용하지 않는 것이 중요합니다.

최소 `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) 값은 `1`입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 프로젝트 전체에서 값의 고유 식별자. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


숫자 또는 비용 값을 나타내는 데 사용되는 실제 값을 설정합니다.

--------------------

Number 또는 Cost 값을 설정해야 할 때, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))보다 이 속성을 사용하는 것이 좋습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | 숫자 또는 비용 값을 나타내는 실제 값. |

### setPhonetic(String value) {#setPhonetic-java.lang.String-}
```
public final void setPhonetic(String value)
```


사용자 정의 필드 이름에 대한 음성 정보를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 사용자 정의 필드 이름에 대한 음성 정보. |

### setStringValue(String value) {#setStringValue-java.lang.String-}
```
public final void setStringValue(String value)
```


텍스트 문자열을 나타내는 데 사용되는 실제 값을 설정합니다.

--------------------

Text 값을 설정해야 할 때, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))보다 이 속성을 사용하는 것이 좋습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 텍스트 문자열을 나타내는 실제 값. |

### setVal(String value) {#setVal-java.lang.String-}
```
public final void setVal(String value)
```


내부 표현에서 실제 값을 설정합니다. 아래에 나열된 강력히 형식화된 속성을 사용하는 것이 좋습니다.

--------------------

Text 값을 설정하려면 강력히 형식화된 `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)) 속성을 사용하는 것이 좋습니다.

Number 또는 Cost 값을 설정하려면 강력히 형식화된 `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)) 속성을 사용하는 것이 좋습니다.

Date/Start/Finish 값을 설정하려면, 강력히 형식화된 `DateTimeValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) 속성을 사용하는 것이 좋습니다.

Duration 값을 설정하려면 강력히 형식화된 `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)) 속성을 사용하는 것이 좋습니다.

목록에 없는 유형인 경우, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) 속성을 사용하십시오.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 내부 표현의 실제 값. |

