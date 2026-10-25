---
title: "المفتاح"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل مفتاح خاصية لفئة من النوع المحدد."
type: docs
weight: 139
url: /ar/java/com.aspose.tasks/key/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct
```
public class Key<T,K> extends Struct<Key<T,K>>
```

يمثل مفتاح خاصية لفئة من النوع المحدد. يُستخدم مثال من هذه الفئة عند الحصول على خاصية أو تعيينها في حاوية.

T : نوع قيمة الخاصية.
K : نوع مفتاح الخاصية.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [Clone()](#Clone--) | يعيد نسخة عميقة من المثيل. |
| [CloneTo(Key&lt;T,K&gt; that)](#CloneTo-com.aspose.tasks.Key-T-K--) | يصنع نسخة عميقة من المثيل إلى مثيل آخر. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Key obj1, Key obj2)](#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-) | يرجع قيمة تشير إلى ما إذا كان المثيل `obj1` المحدد مساويًا للمثيل `obj2` المحدد. |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getKeyType()](#getKeyType--) | يحصل على مفتاح الخاصية. |
| [hashCode()](#hashCode--) | يعيد رمز تجزئة (hash code) لمثيل فئة المفتاح. |
### Clone() {#Clone--}
```
public Key<T,K> Clone()
```


يعيد نسخة عميقة من المثيل.

**Returns:**
[Key](../../com.aspose.tasks/key) - deep copy of the instance.
### CloneTo(Key&lt;T,K&gt; that) {#CloneTo-com.aspose.tasks.Key-T-K--}
```
public void CloneTo(Key<T,K> that)
```


يصنع نسخة عميقة من المثيل إلى مثيل آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| that | [Key](../../com.aspose.tasks/key) | مثال آخر. |

### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### equals(Key obj1, Key obj2) {#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-}
```
public static boolean equals(Key obj1, Key obj2)
```


يرجع قيمة تشير إلى ما إذا كان المثيل `obj1` المحدد مساويًا للمثيل `obj2` المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj1 | com.aspose.tasks.Key | الكائن الأول للمقارنة. |
| obj2 | com.aspose.tasks.Key | الكائن الثاني للمقارنة. |

**Returns:**
boolean - تُرجِع true إذا كان المثال المحدد `obj1` يساوي المثال المحدد `obj2`؛ وإلا، false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
منطقي - \{@inheritDoc\}
### getKeyType() {#getKeyType--}
```
public final K getKeyType()
```


يحصل على مفتاح الخاصية.

**Returns:**
K - مفتاح الخاصية.
### hashCode() {#hashCode--}
```
public int hashCode()
```


يعيد رمز تجزئة (hash code) لمثيل فئة المفتاح.

**Returns:**
int - يعيد رمز تجزئة لهذا الكائن.
