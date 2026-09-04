---
title: "Duration"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل المدة في مشروع."
type: docs
weight: 76
url: /ar/java/com.aspose.tasks/duration/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class Duration extends Struct<Duration> implements System.IEquatable<Duration>
```

يمثل المدة في مشروع.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Duration()](#Duration--) | ينشئ نسخة جديدة من بنية [Duration](../../com.aspose.tasks/duration) باستخدام قيمة TimeSpan محددة وTimeUnitType. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [Clone()](#Clone--) | ينشئ ويُعيد نسخة عميقة من هذا المثيل. |
| [CloneTo(Duration that)](#CloneTo-com.aspose.tasks.Duration-) | يصنع نسخة عميقة من المثيل إلى مثيل آخر. |
| [add(Duration d)](#add-com.aspose.tasks.Duration-) | يضيف المدة المحددة إلى هذه المدة. |
| [add(double val)](#add-double-) | يضيف القيمة المزدوجة المحددة إلى هذه المدة. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [convert(byte timeUnitType)](#convert-byte-) | يحول كائن Duration إلى مدة أخرى باستخدام وحدات زمنية محددة. |
| [equals(Duration other)](#equals-com.aspose.tasks.Duration-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [equals(Duration obj1, Duration obj2)](#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | يرجع قيمة تشير إلى ما إذا كان المثيل `obj1` المحدد مساويًا للمثيل `obj2` المحدد. |
| [equals(Object obj)](#equals-java.lang.Object-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [getTimeSpan()](#getTimeSpan--) | يحصل على نسخة `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) من هذا الكائن Duration. |
| [getTimeUnit()](#getTimeUnit--) | يحصل على نوع وحدة الوقت لهذا الكائن. |
| [hashCode()](#hashCode--) | يعيد قيمة رمز التجزئة لهذا الكائن. |
| [isElapsed()](#isElapsed--) | يحصل على قيمة تشير إلى ما إذا كانت وحدة الوقت منقضية. |
| [isEstimated()](#isEstimated--) | يحصل على قيمة تشير إلى ما إذا كانت وحدة الوقت مقدرة. |
| [op_Equality(Duration a, Duration b)](#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [op_Inequality(Duration a, Duration b)](#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة غير مساوية لكائن محدد. |
| [parse(Project p, String value)](#parse-com.aspose.tasks.Project-java.lang.String-) | يحوّل السلسلة المحددة إلى نسخة من بنية [Duration](../../com.aspose.tasks/duration). |
| [parseTimeSpan(String value)](#parseTimeSpan-java.lang.String-) | يفكك سلسلة المدة بالتنسيق "PT--H--M--S--". |
| [subtract(Duration d)](#subtract-com.aspose.tasks.Duration-) | يطرح المدة المحددة من نسخة هذه المدة. |
| [subtract(double val)](#subtract-double-) | يطرح القيمة العشرية المحددة من نسخة هذه المدة. |
| [toDouble()](#toDouble--) | يحوّل كائن Duration إلى قيمة `double`. |
| [toString()](#toString--) | يعيد تمثيلًا نصيًا لهذه النسخة. |
### Duration() {#Duration--}
```
public Duration()
```


ينشئ نسخة جديدة من بنية [Duration](../../com.aspose.tasks/duration) باستخدام قيمة TimeSpan محددة وTimeUnitType.

### Clone() {#Clone--}
```
public Duration Clone()
```


ينشئ ويُعيد نسخة عميقة من هذا المثيل.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a deep copy of this object.
### CloneTo(Duration that) {#CloneTo-com.aspose.tasks.Duration-}
```
public void CloneTo(Duration that)
```


يصنع نسخة عميقة من المثيل إلى مثيل آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| that | [Duration](../../com.aspose.tasks/duration) | مثال آخر. |

### add(Duration d) {#add-com.aspose.tasks.Duration-}
```
public final Duration add(Duration d)
```


يضيف المدة المحددة إلى هذه المدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | الـ [Duration](../../com.aspose.tasks/duration) المحدد لإضافته إلى هذه النسخة. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### add(double val) {#add-double-}
```
public final Duration add(double val)
```


يضيف القيمة المزدوجة المحددة إلى هذه المدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | القيمة `double` المحددة لإضافتها إلى هذه النسخة. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### convert(byte timeUnitType) {#convert-byte-}
```
public final Duration convert(byte timeUnitType)
```


يحول كائن Duration إلى مدة أخرى باستخدام وحدات زمنية محددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| timeUnitType | byte | نوع وحدة الوقت المحدد. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - returns new duration with the specified unit type.
### equals(Duration other) {#equals-com.aspose.tasks.Duration-}
```
public final boolean equals(Duration other)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [Duration](../../com.aspose.tasks/duration) | الكائن للمقارنة مع هذا المثيل. |

**Returns:**
منطقي - يعيد **True** إذا كانت نسخة Duration الأخرى لها نفس قيمتي TimeSpan و TimeUnit مثل هذه النسخة؛ وإلا، **false**.
### equals(Duration obj1, Duration obj2) {#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean equals(Duration obj1, Duration obj2)
```


يرجع قيمة تشير إلى ما إذا كان المثيل `obj1` المحدد مساويًا للمثيل `obj2` المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj1 | [Duration](../../com.aspose.tasks/duration) | الكائن الأول للمقارنة. |
| obj2 | [Duration](../../com.aspose.tasks/duration) | الكائن الثاني للمقارنة. |

**Returns:**
boolean - تُرجِع true إذا كان المثال المحدد `obj1` يساوي المثال المحدد `obj2`؛ وإلا، false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | الكائن للمقارنة مع هذا المثيل. |

**Returns:**
منطقي - **True** إذا كان الكائن المحدد هو Duration وله نفس قيمتي TimeSpan و TimeUnit مثل هذه النسخة؛ وإلا، **false**.
### getTimeSpan() {#getTimeSpan--}
```
public final double getTimeSpan()
```


يحصل على نسخة `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) من هذا الكائن Duration.

القيمة: نسخة TimeSpan لهذا الكائن Duration.

**Returns:**
مزدوج - نسخة `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) لهذا الكائن Duration.
### getTimeUnit() {#getTimeUnit--}
```
public final byte getTimeUnit()
```


يحصل على نوع وحدة الوقت لهذا الكائن.

القيمة: نوع وحدة الوقت لهذه النسخة من Duration.

**Returns:**
بايت - نوع وحدة الوقت لهذا الكائن.
### hashCode() {#hashCode--}
```
public int hashCode()
```


يعيد قيمة رمز التجزئة لهذا الكائن.

**Returns:**
عدد صحيح - يعيد قيمة رمز التجزئة لهذه النسخة من المدة.
### isElapsed() {#isElapsed--}
```
public final boolean isElapsed()
```


يحصل على قيمة تشير إلى ما إذا كانت وحدة الوقت منقضية.

القيمة: العلامة التي تحدد ما إذا كانت هذه النسخة من Duration منقضية.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كانت وحدة الوقت منقضية.
### isEstimated() {#isEstimated--}
```
public final boolean isEstimated()
```


يحصل على قيمة تشير إلى ما إذا كانت وحدة الوقت مقدرة.

القيمة: العلامة التي تحدد ما إذا كانت هذه النسخة من Duration مقدرة.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كانت وحدة الوقت مقدرة.
### op_Equality(Duration a, Duration b) {#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Equality(Duration a, Duration b)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | المدة الأولى. |
| b | [Duration](../../com.aspose.tasks/duration) | المدة الثانية. |

**Returns:**
منطقي - قيمة تشير إلى ما إذا كانت هذه المثيلة مساوية لكائن محدد
### op_Inequality(Duration a, Duration b) {#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Inequality(Duration a, Duration b)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة غير مساوية لكائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | المدة الأولى. |
| b | [Duration](../../com.aspose.tasks/duration) | المدة الثانية. |

**Returns:**
منطقي - قيمة تشير إلى ما إذا كانت هذه المثيلة غير مساوية لكائن محدد
### parse(Project p, String value) {#parse-com.aspose.tasks.Project-java.lang.String-}
```
public static Duration parse(Project p, String value)
```


يحوّل السلسلة المحددة إلى نسخة من بنية [Duration](../../com.aspose.tasks/duration).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| p | [Project](../../com.aspose.tasks/project) | الكائن المحدد من فئة [Project](../../com.aspose.tasks/project) لتحويل المدة له. |
| القيمة | java.lang.String | السلسلة المحددة للتحويل. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Returns the converted instance of [Duration](../../com.aspose.tasks/duration) struct.
### parseTimeSpan(String value) {#parseTimeSpan-java.lang.String-}
```
public static double parseTimeSpan(String value)
```


يفكك سلسلة المدة بالتنسيق "PT--H--M--S--".

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | السلسلة المحددة للتحليل. |

**Returns:**
double - يُرجع كائنًا مُحللاً من بنية `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)).
### subtract(Duration d) {#subtract-com.aspose.tasks.Duration-}
```
public final Duration subtract(Duration d)
```


يطرح المدة المحددة من نسخة هذه المدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | الكائن [Duration](../../com.aspose.tasks/duration) المحدد للطرح من هذا الكائن. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### subtract(double val) {#subtract-double-}
```
public final Duration subtract(double val)
```


يطرح القيمة العشرية المحددة من نسخة هذه المدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | القيمة `double` المحددة للطرح من هذا الكائن. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### toDouble() {#toDouble--}
```
public final double toDouble()
```


يحوّل كائن Duration إلى قيمة `double`.

**Returns:**
double - القيمة المحوّلة.
### toString() {#toString--}
```
public String toString()
```


يعيد تمثيلًا نصيًا لهذه النسخة.

**Returns:**
java.lang.String - تمثيل نصي لهذا الكائن.
