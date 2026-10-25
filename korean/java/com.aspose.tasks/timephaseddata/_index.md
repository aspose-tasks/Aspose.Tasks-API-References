---
title: "TimephasedData"
second_title: "Aspose.Tasks for Java API Reference"
description: "시간 단계 데이터를 나타냅니다."
type: docs
weight: 320
url: /ko/java/com.aspose.tasks/timephaseddata/
---

**Inheritance:**
java.lang.Object
```
public class TimephasedData
```

시간 단계 데이터를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TimephasedData()](#TimephasedData--) | 새로운 [TimephasedData](../../com.aspose.tasks/timephaseddata) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-) | 비용 기반 시간 분할 데이터용 새로운 [TimephasedData](../../com.aspose.tasks/timephaseddata) 클래스 인스턴스를 생성하고 초기화합니다. |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | 비용 기반 시간 분할 데이터용 새로운 [TimephasedData](../../com.aspose.tasks/timephaseddata) 클래스 인스턴스를 생성하고 초기화합니다. |
| [createUnitTimephased(int uid, Date start, Date finish, double units, byte type)](#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-) | 자재 리소스 할당의 단위 기반 시간 분할 데이터용 새로운 [TimephasedData](../../com.aspose.tasks/timephaseddata) 클래스 인스턴스를 생성하고 초기화합니다. |
| [createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | 작업 기반 시간 분할 데이터용 새로운 [TimephasedData](../../com.aspose.tasks/timephaseddata) 클래스 인스턴스를 생성하고 초기화합니다. |
| [getFinish()](#getFinish--) | 시간 분할 데이터 기간의 종료 날짜를 가져옵니다. |
| [getStart()](#getStart--) | 시간 분할 데이터 기간의 시작 날짜를 가져옵니다. |
| [getTimephasedDataType()](#getTimephasedDataType--) | 시간 분할 데이터의 유형을 가져옵니다. |
| [getUid()](#getUid--) | 시간 분할 데이터의 고유 식별자를 가져옵니다. |
| [getUnit()](#getUnit--) | 시간 분할 데이터 기간의 시간 단위를 가져옵니다. |
| [getValue()](#getValue--) | 시간 분할 데이터 기간의 시간당 값을 가져옵니다. |
| [getValueToCost()](#getValueToCost--) | 이 객체의 문자열 값을 나타내는 `double` 인스턴스를 가져옵니다. |
| [getValueToDuration()](#getValueToDuration--) | 이 객체의 문자열 값을 나타내는 double 인스턴스를 가져옵니다. |
| [getValueToUnits()](#getValueToUnits--) | 단위 기반 시간 단계 데이터에 대한 이 객체의 문자열 값을 나타내는 `double` 인스턴스를 가져옵니다. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | 시간 단계 데이터 기간의 종료 날짜를 설정합니다. |
| [setStart(Date value)](#setStart-java.util.Date-) | 시간 단계 데이터 기간의 시작 날짜를 설정합니다. |
| [setTimephasedDataType(byte value)](#setTimephasedDataType-byte-) | 시간 단계 데이터의 유형을 설정합니다. |
| [setUid(int value)](#setUid-int-) | 시간 단계 데이터의 고유 식별자를 설정합니다 |
| [setUnit(byte value)](#setUnit-byte-) | 시간 단계 데이터 기간의 시간 단위를 설정합니다. |
| [setValue(String value)](#setValue-java.lang.String-) | 시간 단계 데이터 기간에 대한 시간당 값을 설정합니다. |
| [setValueToCost(double value)](#setValueToCost-double-) | `double` 인스턴스는 이 객체의 문자열 값을 나타냅니다. |
### TimephasedData() {#TimephasedData--}
```
public TimephasedData()
```


새로운 [TimephasedData](../../com.aspose.tasks/timephaseddata) 클래스 인스턴스를 초기화합니다.

### createCostTimephased(int uid, Date start, Date finish, double value, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte type)
```


비용 기반 시간 분할 데이터용 새로운 [TimephasedData](../../com.aspose.tasks/timephaseddata) 클래스 인스턴스를 생성하고 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| uid | int | 작업의 UID. |
| 시작 | java.util.Date | 시작 날짜-시간. |
| 완료 | java.util.Date | 종료 날짜-시간. |
| 값 | double | 비용 값. |
| type | 바이트 | 시간 단계 데이터 유형. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


비용 기반 시간 분할 데이터용 새로운 [TimephasedData](../../com.aspose.tasks/timephaseddata) 클래스 인스턴스를 생성하고 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| uid | int | 작업의 UID. |
| 시작 | java.util.Date | 시작 날짜-시간. |
| 완료 | java.util.Date | 종료 날짜-시간. |
| 값 | double | 비용 값. |
| 시간 단위 | 바이트 | 시간 단위 유형. |
| type | 바이트 | 시간 단계 데이터 유형. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createUnitTimephased(int uid, Date start, Date finish, double units, byte type) {#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createUnitTimephased(int uid, Date start, Date finish, double units, byte type)
```


자재 리소스 할당의 단위 기반 시간 분할 데이터용 새로운 [TimephasedData](../../com.aspose.tasks/timephaseddata) 클래스 인스턴스를 생성하고 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| uid | int | 작업의 UID. |
| 시작 | java.util.Date | 시작 날짜-시간. |
| 완료 | java.util.Date | 종료 날짜-시간. |
| 단위 | double | 단위 수. |
| type | 바이트 | 시간 단계 데이터 유형. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


작업 기반 시간 분할 데이터용 새로운 [TimephasedData](../../com.aspose.tasks/timephaseddata) 클래스 인스턴스를 생성하고 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| uid | int | 작업의 UID. |
| 시작 | java.util.Date | 시작 날짜-시간. |
| 완료 | java.util.Date | 종료 날짜-시간. |
| 값 | double | 시간 간격 값. |
| 시간 단위 | 바이트 | 시간 단위 유형. |
| type | 바이트 | 시간 단계 데이터 유형. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


시간 분할 데이터 기간의 종료 날짜를 가져옵니다.

**Returns:**
java.util.Date - 시간 단계 데이터 기간의 종료 날짜.
### getStart() {#getStart--}
```
public final Date getStart()
```


시간 분할 데이터 기간의 시작 날짜를 가져옵니다.

**Returns:**
java.util.Date - 시간 단계 데이터 기간의 시작 날짜.
### getTimephasedDataType() {#getTimephasedDataType--}
```
public final byte getTimephasedDataType()
```


시간 분할 데이터의 유형을 가져옵니다.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) 속성은 여기 지정된 유형에 적합하지 않은 경우 지워집니다.

**Returns:**
byte - 시간 단계 데이터의 유형.
### getUid() {#getUid--}
```
public final int getUid()
```


시간 분할 데이터의 고유 식별자를 가져옵니다.

**Returns:**
int - 시간 단계 데이터의 고유 식별자
### getUnit() {#getUnit--}
```
public final byte getUnit()
```


시간 분할 데이터 기간의 시간 단위를 가져옵니다.

**Returns:**
byte - 시간 단계 데이터 기간의 시간 단위.
### getValue() {#getValue--}
```
public final String getValue()
```


시간 분할 데이터 기간의 시간당 값을 가져옵니다.

**Returns:**
java.lang.String - 시간 단계 데이터 기간당 단위 시간당 값.
### getValueToCost() {#getValueToCost--}
```
public final double getValueToCost()
```


이 객체의 문자열 값을 나타내는 `double` 인스턴스를 가져옵니다.

**Returns:**
double - 객체의 부동 소수점 표현.
### getValueToDuration() {#getValueToDuration--}
```
public final double getValueToDuration()
```


이 객체의 문자열 값을 나타내는 double 인스턴스를 가져옵니다.

**Returns:**
double - 객체의 시간 간격 표현.
### getValueToUnits() {#getValueToUnits--}
```
public final double getValueToUnits()
```


단위 기반 시간 단계 데이터에 대한 이 객체의 문자열 값을 나타내는 `double` 인스턴스를 가져옵니다.

**Returns:**
double - 이 객체의 부동 소수점 표현.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


시간 단계 데이터 기간의 종료 날짜를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 시간 단계 데이터 기간의 종료 날짜. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


시간 단계 데이터 기간의 시작 날짜를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 시간 단계 데이터 기간의 시작 날짜. |

### setTimephasedDataType(byte value) {#setTimephasedDataType-byte-}
```
public final void setTimephasedDataType(byte value)
```


시간 단계 데이터의 유형을 설정합니다.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) 속성은 여기 지정된 유형에 적합하지 않은 경우 지워집니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | 바이트 | 시간 단계 데이터의 유형. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


시간 단계 데이터의 고유 식별자를 설정합니다

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 시간 단계 데이터의 고유 식별자 |

### setUnit(byte value) {#setUnit-byte-}
```
public final void setUnit(byte value)
```


시간 단계 데이터 기간의 시간 단위를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | 바이트 | 시간 단계 데이터 기간의 시간 단위. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


시간 단계 데이터 기간에 대한 시간당 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 시간 단계 데이터 기간당 단위 시간당 값. |

### setValueToCost(double value) {#setValueToCost-double-}
```
public final void setValueToCost(double value)
```


`double` 인스턴스는 이 객체의 문자열 값을 나타냅니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | `double` 인스턴스는 이 객체의 문자열 값을 나타냅니다. |

