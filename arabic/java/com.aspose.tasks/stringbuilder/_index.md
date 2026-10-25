---
title: "StringBuilder"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل سلسلة قابلة للتغيير من الأحرف."
type: docs
weight: 281
url: /ar/java/com.aspose.tasks/stringbuilder/
---

**Inheritance:**
java.lang.Object
```
public final class StringBuilder
```

يمثل سلسلة قابلة للتغيير من الأحرف. لا يمكن تمديده.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [StringBuilder()](#StringBuilder--) | ينشئ نسخة جديدة من فئة StringBuilder. |
| [StringBuilder(int capacity)](#StringBuilder-int-) | ينشئ نسخة جديدة من فئة StringBuilder باستخدام السعة المحددة. |
| [StringBuilder(int capacity, int maxCapacity)](#StringBuilder-int-int-) | ينشئ نسخة جديدة من فئة StringBuilder تبدأ بسعة محددة ويمكن أن تنمو إلى الحد الأقصى المحدد. |
| [StringBuilder(String value)](#StringBuilder-java.lang.String-) | ينشئ نسخة جديدة من فئة StringBuilder باستخدام السلسلة المحددة. |
| [StringBuilder(String value, int capacity)](#StringBuilder-java.lang.String-int-) | ينشئ نسخة جديدة من فئة StringBuilder باستخدام السلسلة والسعة المحددة. |
| [StringBuilder(String value, int startIndex, int length, int capacity)](#StringBuilder-java.lang.String-int-int-int-) | ينشئ نسخة جديدة من فئة StringBuilder من الجزء الفرعي المحدد والسعة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [append(boolean value)](#append-boolean-) | يضيف تمثيل السلسلة لقيمة منطقية محددة إلى هذه النسخة. |
| [append(byte value)](#append-byte-) | يضيف تمثيل السلسلة لبايت محدد إلى هذه النسخة. |
| [append(char value)](#append-char-) | يضيف تمثيل السلسلة لحرف Unicode محدد إلى هذه النسخة. |
| [append(char value, int repeatCount)](#append-char-int-) | يضيف عددًا محددًا من النسخ من تمثيل السلسلة لحرف Unicode إلى هذه النسخة. |
| [append(char[] value)](#append-char---) | يضيف تمثيل السلسلة لأحرف Unicode في مصفوفة محددة إلى هذه النسخة. |
| [append(char[] value, int startIndex, int charCount)](#append-char---int-int-) | يضيف تمثيل السلسلة لمجموعة فرعية محددة من أحرف Unicode إلى هذه النسخة. |
| [append(double value)](#append-double-) | يضيف تمثيل السلسلة لعدد مزدوج محدد إلى هذه النسخة. |
| [append(float value)](#append-float-) | يضيف تمثيل السلسلة لعدد عائم محدد إلى هذه النسخة. |
| [append(int value)](#append-int-) | يضيف تمثيل السلسلة لعدد صحيح محدد إلى هذه النسخة. |
| [append(Object value)](#append-java.lang.Object-) | يضيف تمثيل السلسلة لكائن محدد إلى هذه النسخة. |
| [append(String value)](#append-java.lang.String-) | يضيف نسخة من السلسلة المحددة إلى هذه النسخة. |
| [append(String value, int startIndex, int count)](#append-java.lang.String-int-int-) | يضيف نسخة من جزء فرعي محدد إلى هذه النسخة. |
| [append(BigDecimal value)](#append-java.math.BigDecimal-) | يضيف تمثيل السلسلة لعدد BigDecimal محدد إلى هذه النسخة. |
| [append(long value)](#append-long-) | يضيف تمثيل السلسلة لعدد طويل محدد إلى هذه المثيلة. |
| [append(short value)](#append-short-) | يضيف تمثيل السلسلة لعدد قصير محدد إلى هذه المثيلة. |
| [appendFormat(String format, Object[] args)](#appendFormat-java.lang.String-java.lang.Object...-) | يضيف السلسلة التي تم إرجاعها نتيجة معالجة سلسلة تنسيق مركبة، والتي تحتوي على صفر أو أكثر من عناصر التنسيق، إلى هذه المثيلة. |
| [appendLine()](#appendLine--) | يضيف محدد السطر الافتراضي إلى نهاية كائن StringBuilder الحالي. |
| [appendLine(String value)](#appendLine-java.lang.String-) | يضيف نسخة من السلسلة المحددة متبوعة بمحدد السطر الافتراضي إلى نهاية كائن StringBuilder الحالي. |
| [copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)](#copyTo-int-char---int-int-) | ينسخ الأحرف من جزء محدد من هذه المثيلة إلى جزء محدد من مصفوفة Char الوجهة. |
| [ensureCapacity(int capacity)](#ensureCapacity-int-) | يضمن أن سعة هذه المثيلة من StringBuilder لا تقل عن القيمة المحددة. |
| [equals(Object obj)](#equals-java.lang.Object-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [getCapacity()](#getCapacity--) | يحصل على الحد الأقصى لعدد الأحرف التي يمكن أن تُحتوى في الذاكرة المخصصة للمثيلة الحالية. |
| [getLength()](#getLength--) | يحصل على طول كائن StringBuilder الحالي. |
| [getMaxCapacity()](#getMaxCapacity--) | يحصل على السعة القصوى لهذه المثيلة. |
| [hashCode()](#hashCode--) | يرجع رمز تجزئة لهذا StringBuilder. |
| [insert(int index, boolean value)](#insert-int-boolean-) | يدرج تمثيل السلسلة لقيمة منطقية في هذه المثيلة عند الموضع الحرفي المحدد. |
| [insert(int index, byte value)](#insert-int-byte-) | يدرج تمثيل السلسلة لقيمة بايت في هذه المثيلة عند الموضع الحرفي المحدد. |
| [insert(int index, char value)](#insert-int-char-) | يدرج تمثيل السلسلة لحرف Unicode محدد في هذه المثيلة عند الموضع الحرفي المحدد. |
| [insert(int index, char[] value)](#insert-int-char---) | يدرج تمثيل السلسلة لمصفوفة محددة من أحرف Unicode في هذه المثيلة عند الموضع الحرفي المحدد. |
| [insert(int index, char[] value, int startIndex, int charCount)](#insert-int-char---int-int-) | يدرج تمثيل السلسلة لمجموعة فرعية محددة من أحرف Unicode في هذه المثيلة عند الموضع الحرفي المحدد. |
| [insert(int index, double value)](#insert-int-double-) | يدرج تمثيل السلسلة لعدد مزدوج في هذه المثيلة عند الموضع الحرفي المحدد. |
| [insert(int index, float value)](#insert-int-float-) | يدرج تمثيل السلسلة لعدد عائم في هذه المثيلة عند الموضع الحرفي المحدد. |
| [insert(int index, int value)](#insert-int-int-) | يدرج تمثيل السلسلة لعدد صحيح (int) في هذه المثيلة عند الموضع الحرفي المحدد. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | يدرج تمثيل السلسلة لكائن في هذه المثيلة عند الموضع الحرفي المحدد. |
| [insert(int index, String value)](#insert-int-java.lang.String-) | يدرج سلسلة في هذه المثيلة عند الموضع الحرفي المحدد. |
| [insert(int index, String value, int count)](#insert-int-java.lang.String-int-) | يدرج نسخة واحدة أو أكثر من سلسلة محددة في هذه المثيلة عند الموضع الحرفي المحدد. |
| [insert(int index, BigDecimal value)](#insert-int-java.math.BigDecimal-) | يدرج تمثيل السلسلة لعدد عشري في هذه المثيلة عند الموضع الحرفي المحدد. |
| [insert(int index, long value)](#insert-int-long-) | يدرج تمثيل السلسلة لعدد طويل في هذه المثيلة عند الموضع الحرفي المحدد. |
| [insert(int index, short value)](#insert-int-short-) | يدرج تمثيل السلسلة لعدد قصير في هذه المثيلة عند الموضع الحرفي المحدد. |
| [remove(int startIndex, int length)](#remove-int-int-) | يزيل النطاق المحدد من الأحرف من هذه المثيلة. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | يستبدل جميع تكرارات حرف محدد في هذه المثيلة بحرف محدد آخر. |
| [replace(char oldValue, char newValue, int startIndex, int count)](#replace-char-char-int-int-) | يستبدل، داخل جزء فرعي من هذه المثيلة، جميع تكرارات حرف محدد بحرف محدد آخر. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | يستبدل جميع تكرارات سلسلة محددة في هذه المثيلة بسلسلة محددة أخرى. |
| [replace(String oldValue, String newValue, int startIndex, int count)](#replace-java.lang.String-java.lang.String-int-int-) | يستبدل، داخل جزء فرعي من هذه المثيلة، جميع تكرارات سلسلة محددة بسلسلة محددة أخرى. |
| [setCapacity(int value)](#setCapacity-int-) | يضبط الحد الأقصى لعدد الأحرف التي يمكن أن تحتويها الذاكرة المخصصة للمثيل الحالي. |
| [setLength(int value)](#setLength-int-) | يضبط طول كائن StringBuilder الحالي. |
| [toString()](#toString--) | يحوّل قيمة هذه المثيلة إلى سلسلة. |
| [toString(int startIndex, int length)](#toString-int-int-) | يحوّل قيمة جزء فرعي من هذه المثيلة إلى سلسلة. |
### StringBuilder() {#StringBuilder--}
```
public StringBuilder()
```


ينشئ نسخة جديدة من فئة StringBuilder.

### StringBuilder(int capacity) {#StringBuilder-int-}
```
public StringBuilder(int capacity)
```


ينشئ نسخة جديدة من فئة StringBuilder باستخدام السعة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| السعة | int | الحجم الابتدائي المقترح لهذه المثيلة. |

### StringBuilder(int capacity, int maxCapacity) {#StringBuilder-int-int-}
```
public StringBuilder(int capacity, int maxCapacity)
```


ينشئ نسخة جديدة من فئة StringBuilder تبدأ بسعة محددة ويمكن أن تنمو إلى الحد الأقصى المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| السعة | int | الحجم الابتدائي المقترح لـ StringBuilder. |
| maxCapacity | int | الحد الأقصى لعدد الأحرف التي يمكن أن تحتويها السلسلة الحالية. |

### StringBuilder(String value) {#StringBuilder-java.lang.String-}
```
public StringBuilder(String value)
```


ينشئ نسخة جديدة من فئة StringBuilder باستخدام السلسلة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | السلسلة المستخدمة لتهيئة قيمة المثيلة. |

### StringBuilder(String value, int capacity) {#StringBuilder-java.lang.String-int-}
```
public StringBuilder(String value, int capacity)
```


ينشئ نسخة جديدة من فئة StringBuilder باستخدام السلسلة والسعة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | السلسلة المستخدمة لتهيئة قيمة المثيلة. |
| السعة | int | الحجم الابتدائي المقترح لـ StringBuilder. |

### StringBuilder(String value, int startIndex, int length, int capacity) {#StringBuilder-java.lang.String-int-int-int-}
```
public StringBuilder(String value, int startIndex, int length, int capacity)
```


ينشئ نسخة جديدة من فئة StringBuilder من الجزء الفرعي المحدد والسعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | السلسلة التي تحتوي على الجزء الفرعي المستخدم لتهيئة قيمة هذه المثيلة. |
| startIndex | int | الموضع داخل القيمة حيث يبدأ الجزء الفرعي. |
| length | int | عدد الأحرف في الجزء الفرعي. |
| السعة | int | الحجم الابتدائي المقترح لـ StringBuilder. |

### append(boolean value) {#append-boolean-}
```
public StringBuilder append(boolean value)
```


يضيف تمثيل السلسلة لقيمة منطقية محددة إلى هذه النسخة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | القيمة المنطقية للإضافة. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(byte value) {#append-byte-}
```
public StringBuilder append(byte value)
```


يضيف تمثيل السلسلة لبايت محدد إلى هذه النسخة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte | القيمة للإضافة. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value) {#append-char-}
```
public StringBuilder append(char value)
```


يضيف تمثيل السلسلة لحرف Unicode محدد إلى هذه النسخة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | char | حرف Unicode للإضافة. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value, int repeatCount) {#append-char-int-}
```
public StringBuilder append(char value, int repeatCount)
```


يضيف عددًا محددًا من النسخ من تمثيل السلسلة لحرف Unicode إلى هذه النسخة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | char | الحرف المراد إلحاقه. |
| repeatCount | int | عدد مرات إلحاق القيمة. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value) {#append-char---}
```
public StringBuilder append(char[] value)
```


يضيف تمثيل السلسلة لأحرف Unicode في مصفوفة محددة إلى هذه النسخة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | char[] | مصفوفة الأحرف المراد إلحاقها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value, int startIndex, int charCount) {#append-char---int-int-}
```
public StringBuilder append(char[] value, int startIndex, int charCount)
```


يضيف تمثيل السلسلة لمجموعة فرعية محددة من أحرف Unicode إلى هذه النسخة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | char[] | مصفوفة أحرف. |
| startIndex | int | الموضع الابتدائي في القيمة. |
| charCount | int | عدد الأحرف المراد إلحاقها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(double value) {#append-double-}
```
public StringBuilder append(double value)
```


يضيف تمثيل السلسلة لعدد مزدوج محدد إلى هذه النسخة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | القيمة للإضافة. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(float value) {#append-float-}
```
public StringBuilder append(float value)
```


يضيف تمثيل السلسلة لعدد عائم محدد إلى هذه النسخة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float | القيمة للإضافة. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(int value) {#append-int-}
```
public StringBuilder append(int value)
```


يضيف تمثيل السلسلة لعدد صحيح محدد إلى هذه النسخة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | القيمة للإضافة. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(Object value) {#append-java.lang.Object-}
```
public StringBuilder append(Object value)
```


يضيف تمثيل السلسلة لكائن محدد إلى هذه النسخة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object | الكائن المراد إلحاقه. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value) {#append-java.lang.String-}
```
public StringBuilder append(String value)
```


يضيف نسخة من السلسلة المحددة إلى هذه النسخة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | السلسلة المراد إلحاقها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value, int startIndex, int count) {#append-java.lang.String-int-int-}
```
public StringBuilder append(String value, int startIndex, int count)
```


يضيف نسخة من جزء فرعي محدد إلى هذه النسخة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | السلسلة التي تحتوي على الجزء الفرعي المراد إلحاقه. |
| startIndex | int | الموضع الابتدائي للجزء الفرعي داخل القيمة. |
| count | int | عدد الأحرف في القيمة المراد إلحاقها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(BigDecimal value) {#append-java.math.BigDecimal-}
```
public StringBuilder append(BigDecimal value)
```


يضيف تمثيل السلسلة لعدد BigDecimal محدد إلى هذه النسخة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | القيمة للإضافة. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(long value) {#append-long-}
```
public StringBuilder append(long value)
```


يضيف تمثيل السلسلة لعدد طويل محدد إلى هذه المثيلة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | long | القيمة للإضافة. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(short value) {#append-short-}
```
public StringBuilder append(short value)
```


يضيف تمثيل السلسلة لعدد قصير محدد إلى هذه المثيلة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | short | القيمة للإضافة. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendFormat(String format, Object[] args) {#appendFormat-java.lang.String-java.lang.Object...-}
```
public StringBuilder appendFormat(String format, Object[] args)
```


يُضيف السلسلة التي يتم إرجاعها بعد معالجة سلسلة تنسيق مركبة، والتي تحتوي على صفر أو أكثر من عناصر التنسيق، إلى هذا الكائن. يتم استبدال كل عنصر تنسيق بالتمثيل النصي للمعامل المقابل في مصفوفة المعلمات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| format | java.lang.String | سلسلة تنسيق مركبة. |
| args | java.lang.Object[] | مصفوفة من الكائنات للتنسيق. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with format appended. Each format item in format is replaced by the string representation of the corresponding object argument.
### appendLine() {#appendLine--}
```
public StringBuilder appendLine()
```


يضيف محدد السطر الافتراضي إلى نهاية كائن StringBuilder الحالي.

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendLine(String value) {#appendLine-java.lang.String-}
```
public StringBuilder appendLine(String value)
```


يضيف نسخة من السلسلة المحددة متبوعة بمحدد السطر الافتراضي إلى نهاية كائن StringBuilder الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | السلسلة المراد إلحاقها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### copyTo(int sourceIndex, char[] destination, int destinationIndex, int count) {#copyTo-int-char---int-int-}
```
public void copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)
```


ينسخ الأحرف من جزء محدد من هذه المثيلة إلى جزء محدد من مصفوفة Char الوجهة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceIndex | int | الموضع الابتدائي في هذا الكائن الذي سيتم نسخ الأحرف منه. الفهرس يبدأ من الصفر. |
| الوجهة | char[] | المصفوفة التي سيتم نسخ الأحرف إليها. |
| فهرس الوجهة | int | الموضع الابتدائي في الوجهة حيث سيتم نسخ الأحرف. الفهرس يبدأ من الصفر. |
| count | int | عدد الأحرف التي سيتم نسخها. |

### ensureCapacity(int capacity) {#ensureCapacity-int-}
```
public int ensureCapacity(int capacity)
```


يضمن أن سعة هذه المثيلة من StringBuilder لا تقل عن القيمة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| السعة | int | السعة الدنيا لضمانها. |

**Returns:**
int - السعة الجديدة لهذا الكائن.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | كائن للمقارنة مع هذا الكائن، أو null. |

**Returns:**
boolean - true إذا كان هذا الكائن و sb لهما قيم متساوية في السلسلة، السعة، و MaxCapacity؛ وإلا false.
### getCapacity() {#getCapacity--}
```
public int getCapacity()
```


يحصل على الحد الأقصى لعدد الأحرف التي يمكن أن تُحتوى في الذاكرة المخصصة للمثيلة الحالية.

**Returns:**
int - الحد الأقصى لعدد الأحرف التي يمكن أن تحتويها الذاكرة المخصصة لهذا الكائن.
### getLength() {#getLength--}
```
public int getLength()
```


يحصل على طول كائن StringBuilder الحالي.

**Returns:**
int - طول هذا الكائن.
### getMaxCapacity() {#getMaxCapacity--}
```
public int getMaxCapacity()
```


يحصل على السعة القصوى لهذه المثيلة.

**Returns:**
int - الحد الأقصى لعدد الأحرف التي يمكن لهذا الكائن أن يحملها.
### hashCode() {#hashCode--}
```
public int hashCode()
```


يرجع رمز تجزئة لهذا StringBuilder.

**Returns:**
int - إرجاع قيمة تجزئة لهذا الكائن.
### insert(int index, boolean value) {#insert-int-boolean-}
```
public StringBuilder insert(int index, boolean value)
```


يدرج تمثيل السلسلة لقيمة منطقية في هذه المثيلة عند الموضع الحرفي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الموضع في هذا الكائن حيث يبدأ الإدراج. |
| القيمة | منطقي | القيمة المراد إدراجها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, byte value) {#insert-int-byte-}
```
public StringBuilder insert(int index, byte value)
```


يدرج تمثيل السلسلة لقيمة بايت في هذه المثيلة عند الموضع الحرفي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الموضع في هذا الكائن حيث يبدأ الإدراج. |
| القيمة | byte | القيمة المراد إدراجها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char value) {#insert-int-char-}
```
public StringBuilder insert(int index, char value)
```


يدرج تمثيل السلسلة لحرف Unicode محدد في هذه المثيلة عند الموضع الحرفي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الموضع في هذا الكائن حيث يبدأ الإدراج. |
| القيمة | char | القيمة المراد إدراجها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value) {#insert-int-char---}
```
public StringBuilder insert(int index, char[] value)
```


يدرج تمثيل السلسلة لمصفوفة محددة من أحرف Unicode في هذه المثيلة عند الموضع الحرفي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الموضع في هذا الكائن حيث يبدأ الإدراج. |
| القيمة | char[] | مصفوفة الأحرف المراد إدراجها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value, int startIndex, int charCount) {#insert-int-char---int-int-}
```
public StringBuilder insert(int index, char[] value, int startIndex, int charCount)
```


يدرج تمثيل السلسلة لمجموعة فرعية محددة من أحرف Unicode في هذه المثيلة عند الموضع الحرفي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الموضع في هذا الكائن حيث يبدأ الإدراج. |
| القيمة | char[] | مصفوفة أحرف. |
| startIndex | int | الفهرس الابتدائي داخل القيمة. |
| charCount | int | عدد الأحرف المراد إدراجها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, double value) {#insert-int-double-}
```
public StringBuilder insert(int index, double value)
```


يدرج تمثيل السلسلة لعدد مزدوج في هذه المثيلة عند الموضع الحرفي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الموضع في هذا الكائن حيث يبدأ الإدراج. |
| القيمة | double | القيمة المراد إدراجها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, float value) {#insert-int-float-}
```
public StringBuilder insert(int index, float value)
```


يدرج تمثيل السلسلة لعدد عائم في هذه المثيلة عند الموضع الحرفي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الموضع في هذا الكائن حيث يبدأ الإدراج. |
| القيمة | float | القيمة المراد إدراجها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, int value) {#insert-int-int-}
```
public StringBuilder insert(int index, int value)
```


يدرج تمثيل السلسلة لعدد صحيح (int) في هذه المثيلة عند الموضع الحرفي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الموضع في هذا الكائن حيث يبدأ الإدراج. |
| القيمة | int | القيمة المراد إدراجها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public StringBuilder insert(int index, Object value)
```


يدرج تمثيل السلسلة لكائن في هذه المثيلة عند الموضع الحرفي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الموضع في هذا الكائن حيث يبدأ الإدراج. |
| القيمة | java.lang.Object | الكائن المراد إدراجها، أو null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value) {#insert-int-java.lang.String-}
```
public StringBuilder insert(int index, String value)
```


يدرج سلسلة في هذه المثيلة عند الموضع الحرفي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الموضع في هذا الكائن حيث يبدأ الإدراج. |
| القيمة | java.lang.String | السلسلة المراد إدراجها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value, int count) {#insert-int-java.lang.String-int-}
```
public StringBuilder insert(int index, String value, int count)
```


يدرج نسخة واحدة أو أكثر من سلسلة محددة في هذه المثيلة عند الموضع الحرفي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الموضع في هذا الكائن حيث يبدأ الإدراج. |
| القيمة | java.lang.String | السلسلة المراد إدراجها. |
| count | int | عدد المرات التي سيتم فيها إدراج القيمة. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after insertion has completed.
### insert(int index, BigDecimal value) {#insert-int-java.math.BigDecimal-}
```
public StringBuilder insert(int index, BigDecimal value)
```


يدرج تمثيل السلسلة لعدد عشري في هذه المثيلة عند الموضع الحرفي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الموضع في هذا الكائن حيث يبدأ الإدراج. |
| القيمة | java.math.BigDecimal | القيمة المراد إدراجها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, long value) {#insert-int-long-}
```
public StringBuilder insert(int index, long value)
```


يدرج تمثيل السلسلة لعدد طويل في هذه المثيلة عند الموضع الحرفي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الموضع في هذا الكائن حيث يبدأ الإدراج. |
| القيمة | long | القيمة المراد إدراجها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, short value) {#insert-int-short-}
```
public StringBuilder insert(int index, short value)
```


يدرج تمثيل السلسلة لعدد قصير في هذه المثيلة عند الموضع الحرفي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الموضع في هذا الكائن حيث يبدأ الإدراج. |
| القيمة | short | القيمة المراد إدراجها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### remove(int startIndex, int length) {#remove-int-int-}
```
public StringBuilder remove(int startIndex, int length)
```


يزيل النطاق المحدد من الأحرف من هذه المثيلة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | int | الموضع الذي يبدأ منه الإزالة في هذا الكائن (مؤشر يبدأ من الصفر). |
| length | int | عدد الأحرف المراد إزالتها. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the remove operation has completed.
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public StringBuilder replace(char oldChar, char newChar)
```


يستبدل جميع تكرارات حرف محدد في هذه المثيلة بحرف محدد آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الحرف القديم | char | الحرف المراد استبداله. |
| الحرف الجديد | char | الحرف الذي يستبدل oldChar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar.
### replace(char oldValue, char newValue, int startIndex, int count) {#replace-char-char-int-int-}
```
public StringBuilder replace(char oldValue, char newValue, int startIndex, int count)
```


يستبدل، داخل جزء فرعي من هذه المثيلة، جميع تكرارات حرف محدد بحرف محدد آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| oldValue | char | الحرف المراد استبداله. |
| newValue | char | الحرف الذي يستبدل oldChar. |
| startIndex | int | الموضع في هذا الكائن حيث يبدأ الجزء الفرعي. |
| count | int | طول الجزء الفرعي. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar in the range from startIndex to startIndex + count -1.
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public StringBuilder replace(String oldValue, String newValue)
```


يستبدل جميع تكرارات سلسلة محددة في هذه المثيلة بسلسلة محددة أخرى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| oldValue | java.lang.String | السلسلة التي سيتم استبدالها. |
| newValue | java.lang.String | السلسلة التي تستبدل oldValue، أو null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue.
### replace(String oldValue, String newValue, int startIndex, int count) {#replace-java.lang.String-java.lang.String-int-int-}
```
public StringBuilder replace(String oldValue, String newValue, int startIndex, int count)
```


يستبدل، داخل جزء فرعي من هذه المثيلة، جميع تكرارات سلسلة محددة بسلسلة محددة أخرى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| oldValue | java.lang.String | السلسلة التي سيتم استبدالها. |
| newValue | java.lang.String | السلسلة التي تستبدل oldValue، أو null. |
| startIndex | int | الموضع في هذا الكائن حيث يبدأ الجزء الفرعي. |
| count | int | طول الجزء الفرعي. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue in the range from startIndex to startIndex + count - 1.
### setCapacity(int value) {#setCapacity-int-}
```
public void setCapacity(int value)
```


يضبط الحد الأقصى لعدد الأحرف التي يمكن أن تحتويها الذاكرة المخصصة للمثيل الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | الحد الأقصى لعدد الأحرف التي يمكن أن تحتويها الذاكرة المخصصة لهذا الكائن الحالي. |

### setLength(int value) {#setLength-int-}
```
public void setLength(int value)
```


يضبط طول كائن StringBuilder الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | طول هذا الكائن. |

### toString() {#toString--}
```
public String toString()
```


يحوّل قيمة هذه المثيلة إلى سلسلة.

**Returns:**
java.lang.String - سلسلة قيمتها هي نفسها هذا الكائن.
### toString(int startIndex, int length) {#toString-int-int-}
```
public String toString(int startIndex, int length)
```


يحوّل قيمة جزء فرعي من هذه المثيلة إلى سلسلة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | int | الموضع الابتدائي للجزء الفرعي في هذا الكائن. |
| length | int | طول الجزء الفرعي. |

**Returns:**
java.lang.String - سلسلة قيمتها هي نفسها الجزء الفرعي المحدد لهذا الكائن.
