---
title: "OutlineValue"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir taslak değerini temsil eder."
type: docs
weight: 173
url: /tr/java/com.aspose.tasks/outlinevalue/
---

**Inheritance:**
java.lang.Object
```
public class OutlineValue
```

Bir taslak değerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [OutlineValue()](#OutlineValue--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getDescription()](#getDescription--) | Bir outline değerinin açıklamasını alır. |
| [getDurationValue()](#getDurationValue--) | Tür Duration ise süresi alır. |
| [getParentValueId()](#getParentValueId--) | Bir outline kodunun üst düğümünün kimliğini alır. |
| [getType()](#getType--) | Outline kod türünü alır. |
| [getValue()](#getValue--) | Gerçek değeri alır. |
| [getValueGuid()](#getValueGuid--) | Tüm projedeki diğer değerler arasında bu değeri tanımlayan bir GUID alır. |
| [getValueId()](#getValueId--) | Bir proje içindeki outline kod değerinin benzersiz kimliğini alır. |
| [isCollapsed()](#isCollapsed--) | Outline değerinin daraltılmış olup olmadığını gösteren bir değeri alır. |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | Outline değerinin daraltılmış olup olmadığını gösteren bir değeri ayarlar. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Bir outline değerinin açıklamasını ayarlar. |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Tür Duration ise süresini ayarlar. |
| [setParentValueId(int value)](#setParentValueId-int-) | Bir outline kodunun üst düğümünün kimliğini ayarlar. |
| [setType(int value)](#setType-int-) | Outline kod türünü ayarlar. |
| [setValue(String value)](#setValue-java.lang.String-) | Gerçek değeri ayarlar. |
| [setValueId(int value)](#setValueId-int-) | Bir proje içindeki outline kod değerinin benzersiz kimliğini ayarlar. |
### OutlineValue() {#OutlineValue--}
```
public OutlineValue()
```


### getDescription() {#getDescription--}
```
public final String getDescription()
```


Bir outline değerinin açıklamasını alır.

**Returns:**
java.lang.String - bir outline değerinin açıklaması.
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Tür Duration ise süresi alır.

--------------------

Bu özelliği `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)) yerine tercih edin, Duration türündeki OutlineValues için değeri ayarlamanız gerektiğinde.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration if Type is Duration.
### getParentValueId() {#getParentValueId--}
```
public final int getParentValueId()
```


Bir outline kodunun üst düğümünün kimliğini alır.

**Returns:**
int - bir outline kodunun üst düğümünün kimliği.
### getType() {#getType--}
```
public final int getType()
```


Outline kod türünü alır.

**Returns:**
int - outline kod türü.
### getValue() {#getValue--}
```
public final String getValue()
```


Gerçek değeri alır.

**Returns:**
java.lang.String - gerçek değer.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Tüm projedeki diğer değerler arasında bu değeri tanımlayan bir GUID alır.

**Returns:**
java.util.UUID - tüm projedeki diğer değerler arasında bu değeri tanımlayan bir GUID.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


Bir proje içindeki outline kod değerinin benzersiz kimliğini alır.

**Returns:**
int - bir proje içindeki outline kod değerinin benzersiz kimliği.
### isCollapsed() {#isCollapsed--}
```
public final boolean isCollapsed()
```


Outline değerinin daraltılmış olup olmadığını gösteren bir değeri alır.

--------------------

Bu, MS Project 2010 özelliği için yenidir.

**Returns:**
boolean - outline değerinin daraltılmış olup olmadığını gösteren bir değer.
### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public final void setCollapsed(boolean value)
```


Outline değerinin daraltılmış olup olmadığını gösteren bir değeri ayarlar.

--------------------

Bu, MS Project 2010 özelliği için yenidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | taslak değerinin daraltılmış olup olmadığını gösteren bir değer. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Bir outline değerinin açıklamasını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | bir taslak değerinin açıklaması. |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Tür Duration ise süresini ayarlar.

--------------------

Bu özelliği `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)) yerine tercih edin, Duration türündeki OutlineValues için değeri ayarlamanız gerektiğinde.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Type Duration ise süre. |

### setParentValueId(int value) {#setParentValueId-int-}
```
public final void setParentValueId(int value)
```


Bir outline kodunun üst düğümünün kimliğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | bir taslak kodunun üst düğümünün Id'si. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Outline kod türünü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | taslak kod türü. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Gerçek değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | gerçek değer. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


Bir proje içindeki outline kod değerinin benzersiz kimliğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | bir proje içindeki taslak kod değerinin benzersiz Id'si. |

