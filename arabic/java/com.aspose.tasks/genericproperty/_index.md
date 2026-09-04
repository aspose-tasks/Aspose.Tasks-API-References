---
title: "GenericProperty"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل خاصية الحاوية."
type: docs
weight: 113
url: /ar/java/com.aspose.tasks/genericproperty/
---

**Inheritance:**
java.lang.Object
```
public class GenericProperty<TKey>
```

يمثل خاصية الحاوية.

TKey : نوع قيمة الخاصية.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GenericProperty()](#GenericProperty--) | ينشئ مثيلاً جديداً من الفئة GenericProperty&lt;T&gt;. |
| [GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name)](#GenericProperty-java.lang.Class-TKey--java.lang.String-) | ينشئ مثيلاً جديداً من البنية GenericProperty&lt;TKey&gt;. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [&lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2)](#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--) | يرجع قيمة تشير إلى ما إذا كان المثيل `obj1` المحدد مساويًا للمثيل `obj2` المحدد. |
| [Clone()](#Clone--) | ينشئ ويُعيد نسخة عميقة من هذا المثيل. |
| [CloneTo(GenericProperty&lt;TKey&gt; that)](#CloneTo-com.aspose.tasks.GenericProperty-TKey--) | يصنع نسخة عميقة من المثيل إلى مثيل آخر. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getName()](#getName--) | يحصل على اسم الخاصية. |
| [getValue()](#getValue--) | يحصل على قيمة الخاصية. |
### GenericProperty() {#GenericProperty--}
```
public GenericProperty()
```


ينشئ مثيلاً جديداً من الفئة GenericProperty&lt;T&gt;.

### GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name) {#GenericProperty-java.lang.Class-TKey--java.lang.String-}
```
public GenericProperty(Class<TKey> typeOfTKey, String name)
```


ينشئ مثيلاً جديداً من البنية GenericProperty&lt;TKey&gt;.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| typeOfTKey | java.lang.Class&lt;TKey&gt; |  |
| name | java.lang.String | اسم الخاصية. |

### &lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2) {#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--}
```
public static boolean <TKey>equals(GenericProperty<TKey> obj1, GenericProperty<TKey> obj2)
```


يرجع قيمة تشير إلى ما إذا كان المثيل `obj1` المحدد مساويًا للمثيل `obj2` المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj1 | [GenericProperty](../../com.aspose.tasks/genericproperty) | الكائن الأول للمقارنة. |
| obj2 | [GenericProperty](../../com.aspose.tasks/genericproperty) | الكائن الثاني للمقارنة. |

**Returns:**
boolean - تُرجِع true إذا كان المثال المحدد `obj1` يساوي المثال المحدد `obj2`؛ وإلا، false.
### Clone() {#Clone--}
```
public GenericProperty<TKey> Clone()
```


ينشئ ويُعيد نسخة عميقة من هذا المثيل.

**Returns:**
[GenericProperty](../../com.aspose.tasks/genericproperty) - a deep copy of this object.
### CloneTo(GenericProperty&lt;TKey&gt; that) {#CloneTo-com.aspose.tasks.GenericProperty-TKey--}
```
public void CloneTo(GenericProperty<TKey> that)
```


يصنع نسخة عميقة من المثيل إلى مثيل آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| that | [GenericProperty](../../com.aspose.tasks/genericproperty) | مثال آخر. |

### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
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
### getName() {#getName--}
```
public final String getName()
```


يحصل على اسم الخاصية.

**Returns:**
java.lang.String - اسم الخاصية.
### getValue() {#getValue--}
```
public final Object getValue()
```


يحصل على قيمة الخاصية.

**Returns:**
java.lang.Object - قيمة الخاصية.
