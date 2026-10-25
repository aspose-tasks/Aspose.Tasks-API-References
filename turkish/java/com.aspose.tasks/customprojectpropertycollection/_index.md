---
title: "CustomProjectPropertyCollection"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Özel proje özelliklerinin bir koleksiyonunu temsil eder."
type: docs
weight: 61
url: /tr/java/com.aspose.tasks/customprojectpropertycollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection, com.aspose.tasks.PropertyKeyedCollection
```
public final class CustomProjectPropertyCollection extends PropertyKeyedCollection<CustomProjectProperty>
```

Özel proje özelliklerinin bir koleksiyonunu temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CustomProjectPropertyCollection()](#CustomProjectPropertyCollection--) | Yeni bir [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) sınıf örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | Yeni bir özel özellik oluşturur. |
| [add(String name, double value)](#add-java.lang.String-double-) | Yeni bir özel özellik oluşturur. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Yeni bir özel özellik oluşturur. |
| [add(String name, Date value)](#add-java.lang.String-java.util.Date-) | Yeni bir özel özellik oluşturur. |
| [clear()](#clear--) | PropertyCollection'ı temizler. |
| [isReadOnly()](#isReadOnly--) | Bu koleksiyonun salt okunur olup olmadığını gösteren bir değeri alır; aksi takdirde false. |
| [remove(String name)](#remove-java.lang.String-) | Belirtilen ada sahip bir özelliği koleksiyondan kaldırır. |
### CustomProjectPropertyCollection() {#CustomProjectPropertyCollection--}
```
public CustomProjectPropertyCollection()
```


Yeni bir [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) sınıf örneği başlatır.

### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public final CustomProjectProperty add(String name, boolean value)
```


Yeni bir özel özellik oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String | Özelliğin adı. |
| değer | boolean | Yeni oluşturulan özelliğin nesne değeri. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public final CustomProjectProperty add(String name, double value)
```


Yeni bir özel özellik oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String | Özelliğin adı. |
| değer | double | Yeni oluşturulan özelliğin nesne değeri. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public final CustomProjectProperty add(String name, String value)
```


Yeni bir özel özellik oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String | Özelliğin adı. |
| değer | java.lang.String | Yeni oluşturulan özelliğin nesne değeri. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, Date value) {#add-java.lang.String-java.util.Date-}
```
public final CustomProjectProperty add(String name, Date value)
```


Yeni bir özel özellik oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String | Özelliğin adı. |
| değer | java.util.Date | Yeni oluşturulan özelliğin nesne değeri. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### clear() {#clear--}
```
public final void clear()
```


PropertyCollection'ı temizler.

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Bu koleksiyonun salt okunur olup olmadığını gösteren bir değeri alır; aksi takdirde false.

**Returns:**
boolean - bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer; aksi takdirde false.
### remove(String name) {#remove-java.lang.String-}
```
public final boolean remove(String name)
```


Belirtilen ada sahip bir özelliği koleksiyondan kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String | Özelliğin büyük/küçük harfe duyarsız adı. |

**Returns:**
boolean - Eleman başarıyla bulunup kaldırıldıysa True; aksi takdirde false.
