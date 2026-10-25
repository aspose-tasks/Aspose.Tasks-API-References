---
title: "TimephasedData"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل بيانات زمنية متدرجة."
type: docs
weight: 320
url: /ar/java/com.aspose.tasks/timephaseddata/
---

**Inheritance:**
java.lang.Object
```
public class TimephasedData
```

يمثل بيانات زمنية متدرجة.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [TimephasedData()](#TimephasedData--) | ينشئ مثيلاً جديداً من الفئة [TimephasedData](../../com.aspose.tasks/timephaseddata). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-) | ينشئ ويُهيئ نسخة جديدة من الفئة [TimephasedData](../../com.aspose.tasks/timephaseddata) لبيانات الوقت المرحلية المستندة إلى التكلفة. |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | ينشئ ويُهيئ نسخة جديدة من الفئة [TimephasedData](../../com.aspose.tasks/timephaseddata) لبيانات الوقت المرحلية المستندة إلى التكلفة. |
| [createUnitTimephased(int uid, Date start, Date finish, double units, byte type)](#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-) | ينشئ ويُهيئ نسخة جديدة من الفئة [TimephasedData](../../com.aspose.tasks/timephaseddata) لبيانات الوقت المرحلية المستندة إلى الوحدة لتعيين مورد مادي. |
| [createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | ينشئ ويُهيئ نسخة جديدة من الفئة [TimephasedData](../../com.aspose.tasks/timephaseddata) لبيانات الوقت المرحلية المستندة إلى العمل. |
| [getFinish()](#getFinish--) | يحصل على تاريخ الانتهاء لفترة بيانات الوقت المرحلية. |
| [getStart()](#getStart--) | يحصل على تاريخ البدء لفترة بيانات الوقت المرحلية. |
| [getTimephasedDataType()](#getTimephasedDataType--) | يحصل على نوع بيانات الوقت المرحلية. |
| [getUid()](#getUid--) | يحصل على المعرف الفريد لبيانات الوقت المرحلية |
| [getUnit()](#getUnit--) | يحصل على وحدة الوقت لفترة بيانات الوقت المرحلية. |
| [getValue()](#getValue--) | يحصل على القيمة لكل وحدة زمنية لفترة بيانات الوقت المرحلية. |
| [getValueToCost()](#getValueToCost--) | يحصل على نسخة `double` التي تمثل القيمة النصية لهذا الكائن. |
| [getValueToDuration()](#getValueToDuration--) | يحصل على نسخة double التي تمثل القيمة النصية لهذا الكائن. |
| [getValueToUnits()](#getValueToUnits--) | يحصل على نسخة `double` التي تمثل القيمة النصية لهذا الكائن لبيانات الوقت المرحلية المستندة إلى الوحدة. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | يضبط تاريخ الانتهاء لفترة بيانات الوقت المرحلية. |
| [setStart(Date value)](#setStart-java.util.Date-) | يضبط تاريخ البدء لفترة بيانات الوقت المرحلية. |
| [setTimephasedDataType(byte value)](#setTimephasedDataType-byte-) | يضبط نوع بيانات الوقت المرحلية. |
| [setUid(int value)](#setUid-int-) | يضبط المعرف الفريد لبيانات الوقت المرحلية |
| [setUnit(byte value)](#setUnit-byte-) | يضبط وحدة الوقت لفترة بيانات الوقت المرحلية. |
| [setValue(String value)](#setValue-java.lang.String-) | يضبط القيمة لكل وحدة زمنية لفترة بيانات الوقت المرحلية. |
| [setValueToCost(double value)](#setValueToCost-double-) | نسخة `double` التي تمثل القيمة النصية لهذا الكائن. |
### TimephasedData() {#TimephasedData--}
```
public TimephasedData()
```


ينشئ مثيلاً جديداً من الفئة [TimephasedData](../../com.aspose.tasks/timephaseddata).

### createCostTimephased(int uid, Date start, Date finish, double value, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte type)
```


ينشئ ويُهيئ نسخة جديدة من الفئة [TimephasedData](../../com.aspose.tasks/timephaseddata) لبيانات الوقت المرحلية المستندة إلى التكلفة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | int | معرف فريد للمهمة. |
| بدء | java.util.Date | تاريخ ووقت البدء. |
| الانتهاء | java.util.Date | تاريخ ووقت الانتهاء. |
| القيمة | double | قيمة التكلفة. |
| type | byte | نوع بيانات الوقت المرحلية. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


ينشئ ويُهيئ نسخة جديدة من الفئة [TimephasedData](../../com.aspose.tasks/timephaseddata) لبيانات الوقت المرحلية المستندة إلى التكلفة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | int | معرف فريد للمهمة. |
| بدء | java.util.Date | تاريخ ووقت البدء. |
| الانتهاء | java.util.Date | تاريخ ووقت الانتهاء. |
| القيمة | double | قيمة التكلفة. |
| وحدة الوقت | byte | نوع وحدة الوقت. |
| type | byte | نوع بيانات الوقت المرحلية. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createUnitTimephased(int uid, Date start, Date finish, double units, byte type) {#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createUnitTimephased(int uid, Date start, Date finish, double units, byte type)
```


ينشئ ويُهيئ نسخة جديدة من الفئة [TimephasedData](../../com.aspose.tasks/timephaseddata) لبيانات الوقت المرحلية المستندة إلى الوحدة لتعيين مورد مادي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | int | معرف فريد للمهمة. |
| بدء | java.util.Date | تاريخ ووقت البدء. |
| الانتهاء | java.util.Date | تاريخ ووقت الانتهاء. |
| الوحدات | double | عدد الوحدات. |
| type | byte | نوع بيانات الوقت المرحلية. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


ينشئ ويُهيئ نسخة جديدة من الفئة [TimephasedData](../../com.aspose.tasks/timephaseddata) لبيانات الوقت المرحلية المستندة إلى العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | int | معرف فريد للمهمة. |
| بدء | java.util.Date | تاريخ ووقت البدء. |
| الانتهاء | java.util.Date | تاريخ ووقت الانتهاء. |
| القيمة | double | قيمة فترة الزمن. |
| وحدة الوقت | byte | نوع وحدة الوقت. |
| type | byte | نوع بيانات الوقت المرحلية. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


يحصل على تاريخ الانتهاء لفترة بيانات الوقت المرحلية.

**Returns:**
java.util.Date - تاريخ الانتهاء لفترة بيانات زمنية متدرجة.
### getStart() {#getStart--}
```
public final Date getStart()
```


يحصل على تاريخ البدء لفترة بيانات الوقت المرحلية.

**Returns:**
java.util.Date - تاريخ البدء لفترة بيانات زمنية متدرجة.
### getTimephasedDataType() {#getTimephasedDataType--}
```
public final byte getTimephasedDataType()
```


يحصل على نوع بيانات الوقت المرحلية.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) الخاصية سيتم مسحها إذا لم تكن مناسبة للنوع المحدد هنا.

**Returns:**
byte - نوع بيانات زمنية متدرجة.
### getUid() {#getUid--}
```
public final int getUid()
```


يحصل على المعرف الفريد لبيانات الوقت المرحلية

**Returns:**
int - المعرف الفريد لبيانات زمنية متدرجة
### getUnit() {#getUnit--}
```
public final byte getUnit()
```


يحصل على وحدة الوقت لفترة بيانات الوقت المرحلية.

**Returns:**
byte - وحدة الوقت لفترة بيانات زمنية متدرجة.
### getValue() {#getValue--}
```
public final String getValue()
```


يحصل على القيمة لكل وحدة زمنية لفترة بيانات الوقت المرحلية.

**Returns:**
java.lang.String - القيمة لكل وحدة زمنية لفترة بيانات زمنية متدرجة.
### getValueToCost() {#getValueToCost--}
```
public final double getValueToCost()
```


يحصل على نسخة `double` التي تمثل القيمة النصية لهذا الكائن.

**Returns:**
double - تمثيل بنقطة عائمة للكائن.
### getValueToDuration() {#getValueToDuration--}
```
public final double getValueToDuration()
```


يحصل على نسخة double التي تمثل القيمة النصية لهذا الكائن.

**Returns:**
double - تمثيل فترة زمنية للكائن.
### getValueToUnits() {#getValueToUnits--}
```
public final double getValueToUnits()
```


يحصل على نسخة `double` التي تمثل القيمة النصية لهذا الكائن لبيانات الوقت المرحلية المستندة إلى الوحدة.

**Returns:**
double - تمثيل بنقطة عائمة لهذا الكائن.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


يضبط تاريخ الانتهاء لفترة بيانات الوقت المرحلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | تاريخ الانتهاء لفترة بيانات زمنية متدرجة. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


يضبط تاريخ البدء لفترة بيانات الوقت المرحلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | تاريخ البدء لفترة بيانات زمنية متدرجة. |

### setTimephasedDataType(byte value) {#setTimephasedDataType-byte-}
```
public final void setTimephasedDataType(byte value)
```


يضبط نوع بيانات الوقت المرحلية.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) الخاصية سيتم مسحها إذا لم تكن مناسبة للنوع المحدد هنا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte | نوع بيانات زمنية متدرجة. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


يضبط المعرف الفريد لبيانات الوقت المرحلية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | المعرف الفريد لبيانات زمنية متدرجة |

### setUnit(byte value) {#setUnit-byte-}
```
public final void setUnit(byte value)
```


يضبط وحدة الوقت لفترة بيانات الوقت المرحلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte | وحدة الوقت لفترة بيانات زمنية متدرجة. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


يضبط القيمة لكل وحدة زمنية لفترة بيانات الوقت المرحلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | القيمة لكل وحدة زمنية لفترة بيانات زمنية متدرجة. |

### setValueToCost(double value) {#setValueToCost-double-}
```
public final void setValueToCost(double value)
```


نسخة `double` التي تمثل القيمة النصية لهذا الكائن.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | نسخة `double` التي تمثل القيمة النصية لهذا الكائن. |

