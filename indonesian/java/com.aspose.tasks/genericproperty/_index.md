---
title: "GenericProperty"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili properti kontainer."
type: docs
weight: 113
url: /id/java/com.aspose.tasks/genericproperty/
---

**Inheritance:**
java.lang.Object
```
public class GenericProperty<TKey>
```

Mewakili properti kontainer.

TKey : Tipe nilai properti.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [GenericProperty()](#GenericProperty--) | Menginisialisasi instance baru dari kelas GenericProperty&lt;T&gt;. |
| [GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name)](#GenericProperty-java.lang.Class-TKey--java.lang.String-) | Menginisialisasi instance baru dari struct GenericProperty&lt;TKey&gt;. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [&lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2)](#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--) | Mengembalikan nilai yang menunjukkan apakah instance `obj1` yang ditentukan sama dengan instance `obj2` yang ditentukan. |
| [Clone()](#Clone--) | Membuat dan mengembalikan salinan mendalam dari instance ini. |
| [CloneTo(GenericProperty&lt;TKey&gt; that)](#CloneTo-com.aspose.tasks.GenericProperty-TKey--) | Membuat salinan mendalam dari instance ke instance lain. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getName()](#getName--) | Mendapatkan nama properti. |
| [getValue()](#getValue--) | Mendapatkan nilai properti. |
### GenericProperty() {#GenericProperty--}
```
public GenericProperty()
```


Menginisialisasi instance baru dari kelas GenericProperty&lt;T&gt;.

### GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name) {#GenericProperty-java.lang.Class-TKey--java.lang.String-}
```
public GenericProperty(Class<TKey> typeOfTKey, String name)
```


Menginisialisasi instance baru dari struct GenericProperty&lt;TKey&gt;.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| typeOfTKey | java.lang.Class&lt;TKey&gt; |  |
| name | java.lang.String | Nama properti. |

### &lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2) {#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--}
```
public static boolean <TKey>equals(GenericProperty<TKey> obj1, GenericProperty<TKey> obj2)
```


Mengembalikan nilai yang menunjukkan apakah instance `obj1` yang ditentukan sama dengan instance `obj2` yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj1 | [GenericProperty](../../com.aspose.tasks/genericproperty) | objek pertama untuk dibandingkan. |
| obj2 | [GenericProperty](../../com.aspose.tasks/genericproperty) | objek kedua untuk dibandingkan. |

**Returns:**
boolean - mengembalikan true jika instansi `obj1` yang ditentukan sama dengan instansi `obj2` yang ditentukan; jika tidak, false.
### Clone() {#Clone--}
```
public GenericProperty<TKey> Clone()
```


Membuat dan mengembalikan salinan mendalam dari instance ini.

**Returns:**
[GenericProperty](../../com.aspose.tasks/genericproperty) - a deep copy of this object.
### CloneTo(GenericProperty&lt;TKey&gt; that) {#CloneTo-com.aspose.tasks.GenericProperty-TKey--}
```
public void CloneTo(GenericProperty<TKey> that)
```


Membuat salinan mendalam dari instance ke instance lain.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| that | [GenericProperty](../../com.aspose.tasks/genericproperty) | instansi lain. |

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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getName() {#getName--}
```
public final String getName()
```


Mendapatkan nama properti.

**Returns:**
java.lang.String - nama properti.
### getValue() {#getValue--}
```
public final Object getValue()
```


Mendapatkan nilai properti.

**Returns:**
java.lang.Object - nilai properti.
