---
title: "TimeDelta"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل فرقًا بين طابعين زمنيّين."
type: docs
weight: 317
url: /ar/java/com.aspose.tasks/timedelta/
---

**Inheritance:**
java.lang.Object
```
public class TimeDelta
```

يمثل فرقًا بين طابعين زمنيّين.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [TimeDelta(int hours, int minutes, int seconds)](#TimeDelta-int-int-int-) | يُهيئ مثيلاً جديداً من TimeDelta إلى العدد المحدد من الساعات والدقائق والثواني. |
| [TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)](#TimeDelta-int-int-int-int-int-) | يُهيئ مثيلاً جديداً من TimeDelta إلى العدد المحدد من الأيام والساعات والدقائق والثواني والميليثانية. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(TimeDelta other)](#add-com.aspose.tasks.TimeDelta-) | يعيد كائن TimeDelta جديد تكون قيمته مجموع هذا المثيل والمثيل الآخر. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [compare(TimeDelta t1, TimeDelta t2)](#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | يقارن قيمتي TimeDelta ويعيد عددًا صحيحًا يشير إلى ما إذا كانت القيمة الأولى أقصر من أو مساوية أو أطول من القيمة الثانية. |
| [compareTo(TimeDelta other)](#compareTo-com.aspose.tasks.TimeDelta-) | يقارن هذا المثيل بكائن TimeDelta محدد ويعيد عددًا صحيحًا يشير إلى ما إذا كان هذا المثيل أقصر من أو مساوي أو أطول من كائن TimeSpan. |
| [equals(TimeDelta other)](#equals-com.aspose.tasks.TimeDelta-) | يشير إلى ما إذا كان بعض الفاصل الزمني `other` يساوي هذا. |
| [equals(TimeDelta t1, TimeDelta t2)](#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | يفحص مثيلين للتحقق من المساواة. |
| [equals(Object other)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [fromDays(double value)](#fromDays-double-) | يرجع كائن TimeDelta يمثل عددًا محددًا من الأيام (مقربًا إلى أقرب مللي ثانية). |
| [fromHours(double value)](#fromHours-double-) | يرجع كائن TimeDelta يمثل عددًا محددًا من الساعات (مقربًا إلى أقرب مللي ثانية). |
| [fromMilliseconds(double value)](#fromMilliseconds-double-) | يرجع كائن TimeDelta يمثل عددًا محددًا من المللي ثانية (مقربًا إلى أقرب مللي ثانية). |
| [fromMinutes(double value)](#fromMinutes-double-) | يرجع كائن TimeDelta يمثل عددًا محددًا من الدقائق (مقربًا إلى أقرب مللي ثانية). |
| [fromSeconds(double value)](#fromSeconds-double-) | يرجع كائن TimeDelta يمثل عددًا محددًا من الثواني (مقربًا إلى أقرب مللي ثانية). |
| [getDays()](#getDays--) | يرجع مكوّن الأيام لفترة الوقت، الممثلة بهذا المثيل. |
| [getHours()](#getHours--) | يرجع مكوّن الساعات لفترة الوقت، الممثلة بهذا المثيل. |
| [getMilliseconds()](#getMilliseconds--) | يرجع مكوّن المللي ثانية لفترة الوقت، الممثلة بهذا المثيل. |
| [getMinutes()](#getMinutes--) | يرجع مكوّن الدقائق لفترة الوقت، الممثلة بهذا المثيل. |
| [getSeconds()](#getSeconds--) | يرجع مكوّن الثواني لفترة الوقت، الممثلة بهذا المثيل. |
| [getTotalDays()](#getTotalDays--) | يرجع قيمة المثيل الحالي معبرًا عنها بأيام كاملة وكسرية. |
| [getTotalHours()](#getTotalHours--) | يرجع قيمة المثيل الحالي معبرًا عنها بساعات كاملة وكسرية. |
| [getTotalMilliseconds()](#getTotalMilliseconds--) | يرجع قيمة المثيل الحالي معبرًا عنها بمللي ثوانٍ كاملة وكسرية. |
| [getTotalMinutes()](#getTotalMinutes--) | يرجع قيمة المثيل الحالي معبرًا عنها بدقائق كاملة وكسرية. |
| [getTotalSeconds()](#getTotalSeconds--) | يرجع قيمة المثيل الحالي معبرًا عنها بثوانٍ كاملة وكسرية. |
| [hashCode()](#hashCode--) | \{@inheritDoc\} |
| [negate()](#negate--) | يرجع كائن `TimeDelta` جديد تكون قيمته هي القيمة السالبة لهذا المثيل. |
| [parse(String s)](#parse-java.lang.String-) | يحوّل تمثيل السلسلة لفترة الوقت إلى ما يعادلها من `TimeDelta`. |
| [subtract(TimeDelta other)](#subtract-com.aspose.tasks.TimeDelta-) | يرجع كائن TimeDelta جديد تكون قيمته الفرق بين هذا المثيل و`other`. |
| [toString()](#toString--) | \{@inheritDoc\} |
| [tryParse(String s, TimeDelta[] result)](#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---) | يحوّل تمثيل السلسلة لفترة الوقت إلى ما يعادلها من TimeDelta ويُرجع قيمة تُظهر ما إذا كان التحويل ناجحًا. |
### TimeDelta(int hours, int minutes, int seconds) {#TimeDelta-int-int-int-}
```
public TimeDelta(int hours, int minutes, int seconds)
```


يُهيئ مثيلاً جديداً من TimeDelta إلى العدد المحدد من الساعات والدقائق والثواني.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ساعات | int | عدد الساعات. |
| دقائق | int | عدد الدقائق. |
| ثوانٍ | int | عدد الثواني. |

### TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds) {#TimeDelta-int-int-int-int-int-}
```
public TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)
```


يُهيئ مثيلاً جديداً من TimeDelta إلى العدد المحدد من الأيام والساعات والدقائق والثواني والميليثانية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| أيام | int | عدد الأيام. |
| ساعات | int | عدد الساعات. |
| دقائق | int | عدد الدقائق. |
| ثوانٍ | int | عدد الثواني. |
| ميليثانية | int | عدد الميليثواني. |

### add(TimeDelta other) {#add-com.aspose.tasks.TimeDelta-}
```
public TimeDelta add(TimeDelta other)
```


يعيد كائن TimeDelta جديد تكون قيمته مجموع هذا المثيل والمثيل الآخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | الكائن المراد جمعه. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance plus value of other instance.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### compare(TimeDelta t1, TimeDelta t2) {#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static int compare(TimeDelta t1, TimeDelta t2)
```


يقارن قيمتي TimeDelta ويعيد عددًا صحيحًا يشير إلى ما إذا كانت القيمة الأولى أقصر من أو مساوية أو أطول من القيمة الثانية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | الفاصل الزمني الأول للمقارنة. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | الفاصل الزمني الثاني للمقارنة. |

**Returns:**
int - \-1 إذا كان `t1` أقصر من `t2`، 0 إذا كان `t1` يساوي `t2` و 1 إذا كان `t1` أطول من `t2`.
### compareTo(TimeDelta other) {#compareTo-com.aspose.tasks.TimeDelta-}
```
public int compareTo(TimeDelta other)
```


يقارن هذا المثيل بكائن TimeDelta محدد ويعيد عددًا صحيحًا يشير إلى ما إذا كان هذا المثيل أقصر من أو مساوي أو أطول من كائن TimeSpan.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | كائن للمقارنة معه. |

**Returns:**
int - \-1 إذا كان هذا الكائن أقصر من `other`، 0 إذا كان هذا الكائن يساوي `other` و 1 إذا كان هذا الكائن أطول من `other`.
### equals(TimeDelta other) {#equals-com.aspose.tasks.TimeDelta-}
```
public boolean equals(TimeDelta other)
```


يشير إلى ما إذا كان بعض الفاصل الزمني `other` يساوي هذا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | الفترة الزمنية للمقارنة معها. |

**Returns:**
منطقي - `true` إذا كانت الفواصل متساوية؛ `false` غير ذلك.
### equals(TimeDelta t1, TimeDelta t2) {#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static boolean equals(TimeDelta t1, TimeDelta t2)
```


يفحص مثيلين للتحقق من المساواة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | الكائن الأول. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | الكائن الثاني. |

**Returns:**
منطقي - `true` إذا كانت الكائنات متساوية؛ `false` غير ذلك.
### equals(Object other) {#equals-java.lang.Object-}
```
public boolean equals(Object other)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| آخر | java.lang.Object | \{@inheritDoc\} |

**Returns:**
منطقي - \{@inheritDoc\}
### fromDays(double value) {#fromDays-double-}
```
public static TimeDelta fromDays(double value)
```


يرجع كائن TimeDelta يمثل عددًا محددًا من الأيام (مقربًا إلى أقرب مللي ثانية).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | عدد من الأيام. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromHours(double value) {#fromHours-double-}
```
public static TimeDelta fromHours(double value)
```


يرجع كائن TimeDelta يمثل عددًا محددًا من الساعات (مقربًا إلى أقرب مللي ثانية).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | عدد من الساعات. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMilliseconds(double value) {#fromMilliseconds-double-}
```
public static TimeDelta fromMilliseconds(double value)
```


يرجع كائن TimeDelta يمثل عددًا محددًا من المللي ثانية (مقربًا إلى أقرب مللي ثانية).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | عدد من الميليثواني. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMinutes(double value) {#fromMinutes-double-}
```
public static TimeDelta fromMinutes(double value)
```


يرجع كائن TimeDelta يمثل عددًا محددًا من الدقائق (مقربًا إلى أقرب مللي ثانية).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | عدد من الدقائق. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromSeconds(double value) {#fromSeconds-double-}
```
public static TimeDelta fromSeconds(double value)
```


يرجع كائن TimeDelta يمثل عددًا محددًا من الثواني (مقربًا إلى أقرب مللي ثانية).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | عدد من الثواني. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### getDays() {#getDays--}
```
public int getDays()
```


يرجع مكوّن الأيام لفترة الوقت، الممثلة بهذا المثيل.

**Returns:**
int - مكوّن الأيام في الفاصل الزمني. يمكن أن يكون موجبًا أو سالبًا.
### getHours() {#getHours--}
```
public int getHours()
```


يرجع مكوّن الساعات لفترة الوقت، الممثلة بهذا المثيل.

**Returns:**
int - مكوّن الساعات في الفاصل الزمني في النطاق من -23 إلى 23.
### getMilliseconds() {#getMilliseconds--}
```
public int getMilliseconds()
```


يرجع مكوّن المللي ثانية لفترة الوقت، الممثلة بهذا المثيل.

**Returns:**
int - مكوّن الميليثواني في الفاصل الزمني في النطاق من -999 إلى 999.
### getMinutes() {#getMinutes--}
```
public int getMinutes()
```


يرجع مكوّن الدقائق لفترة الوقت، الممثلة بهذا المثيل.

**Returns:**
int - مكوّن الدقائق لفاصل الوقت في النطاق من -59 إلى 59.
### getSeconds() {#getSeconds--}
```
public int getSeconds()
```


يرجع مكوّن الثواني لفترة الوقت، الممثلة بهذا المثيل.

**Returns:**
int - مكوّن الثواني لفاصل الوقت في النطاق من -59 إلى 59.
### getTotalDays() {#getTotalDays--}
```
public double getTotalDays()
```


يرجع قيمة المثيل الحالي معبرًا عنها بأيام كاملة وكسرية.

**Returns:**
double - إجمالي عدد الأيام التي يمثلها هذا الكائن.
### getTotalHours() {#getTotalHours--}
```
public double getTotalHours()
```


يرجع قيمة المثيل الحالي معبرًا عنها بساعات كاملة وكسرية.

**Returns:**
double - إجمالي عدد الساعات التي يمثلها هذا الكائن.
### getTotalMilliseconds() {#getTotalMilliseconds--}
```
public double getTotalMilliseconds()
```


يرجع قيمة المثيل الحالي معبرًا عنها بمللي ثوانٍ كاملة وكسرية.

**Returns:**
double - إجمالي عدد الملليثواني التي يمثلها هذا الكائن.
### getTotalMinutes() {#getTotalMinutes--}
```
public double getTotalMinutes()
```


يرجع قيمة المثيل الحالي معبرًا عنها بدقائق كاملة وكسرية.

**Returns:**
double - إجمالي عدد الدقائق التي يمثلها هذا الكائن.
### getTotalSeconds() {#getTotalSeconds--}
```
public double getTotalSeconds()
```


يرجع قيمة المثيل الحالي معبرًا عنها بثوانٍ كاملة وكسرية.

**Returns:**
double - إجمالي عدد الثواني التي يمثلها هذا الكائن.
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int - \{@inheritDoc\}
### negate() {#negate--}
```
public TimeDelta negate()
```


يرجع كائن `TimeDelta` جديد تكون قيمته هي القيمة السالبة لهذا المثيل.

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - A new object with the same numeric value as this instance, but with the opposite sign.
### parse(String s) {#parse-java.lang.String-}
```
public static TimeDelta parse(String s)
```


يحوّل تمثيل السلسلة لفترة الوقت إلى ما يعادلها من `TimeDelta`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| s | java.lang.String | سلسلة نصية تحدد فاصل الوقت للتحويل. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a time interval that corresponds to `s`.
### subtract(TimeDelta other) {#subtract-com.aspose.tasks.TimeDelta-}
```
public TimeDelta subtract(TimeDelta other)
```


يرجع كائن TimeDelta جديد تكون قيمته الفرق بين هذا المثيل و`other`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | الكائن المراد طرحه. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance minus value of other instance.
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String - \{@inheritDoc\}
### tryParse(String s, TimeDelta[] result) {#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---}
```
public static boolean tryParse(String s, TimeDelta[] result)
```


يحوّل تمثيل السلسلة لفترة الوقت إلى ما يعادلها من TimeDelta ويُرجع قيمة تُظهر ما إذا كان التحويل ناجحًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| s | java.lang.String | سلسلة نصية تحدد فاصل الوقت للتحويل. |
| result | [TimeDelta\[\]](../../com.aspose.tasks/timedelta) | يجب أن تحتوي هذه المصفوفة على عنصر واحد على الأقل. عندما تعود هذه الطريقة، يحتوي `result[0]` على كائن يمثل فاصل الوقت المحدد بواسطة `s`، أو فاصل وقت بطول صفر إذا فشل التحويل. |

**Returns:**
boolean - `true` إذا تم تحويل s بنجاح؛ وإلا `false`.
