---
title: "GroupCriterion"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir grup tanımındaki ölçütü temsil eder."
type: docs
weight: 124
url: /tr/java/com.aspose.tasks/groupcriterion/
---

**Inheritance:**
java.lang.Object
```
public class GroupCriterion
```

Bir grup tanımında bir kriteri temsil eder. GroupCriterion nesnesi, [GroupCriterionCollection](../../com.aspose.tasks/groupcriterioncollection) koleksiyonunun bir üyesidir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GroupCriterion()](#GroupCriterion--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [getAscending()](#getAscending--) | Bir grup tanımında kriter olarak kullanılan bir alanın artan sırada sıralanıp sıralanmadığını gösteren bir değer alır. |
| [getCellColor()](#getCellColor--) | Bir grup tanımında kriter olarak kullanılan bir alanın hücre arka plan rengini alır. |
| [getField()](#getField--) | Gruplandırılan alanı alır. |
| [getFont()](#getFont--) | Bir grup tanımındaki kriter için yazı tipini alır. |
| [getFontColor()](#getFontColor--) | Bir grup tanımında kriter olarak kullanılan bir alanın yazı tipi rengini alır. |
| [getGroupInterval()](#getGroupInterval--) | Bir grup tanımında kriter olarak kullanılan bir alanın aralığını alır. |
| [getGroupOn()](#getGroupOn--) | Bir grup tanımında kriter olarak kullanılan bir alanın grup türünü alır. |
| [getPattern()](#getPattern--) | Bir grup tanımında kriter olarak kullanılan bir alanın hücre desenini alır. |
| [getStartAt()](#getStartAt--) | Bir grup tanımında kriter olarak kullanılan bir alanın aralık başlangıcını alır. |
| [hashCode()](#hashCode--) | Belirli bir tip için bir karma işlevi olarak hizmet eder. |
| [setAscending(boolean value)](#setAscending-boolean-) | Bir grup tanımında kriter olarak kullanılan bir alanın artan sırada sıralanıp sıralanmadığını gösteren bir değeri ayarlar. |
| [setCellColor(Color value)](#setCellColor-java.awt.Color-) | Bir grup tanımında kriter olarak kullanılan bir alanın hücre arka plan rengini ayarlar. |
| [setField(int value)](#setField-int-) | Gruplandırılan alanı ayarlar. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | Bir grup tanımında kriter için yazı tipini ayarlar. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Bir grup tanımında kriter olarak kullanılan bir alanın yazı tipi rengini ayarlar. |
| [setGroupInterval(Object value)](#setGroupInterval-java.lang.Object-) | Bir grup tanımında kriter olarak kullanılan bir alan için aralığı ayarlar. |
| [setGroupOn(int value)](#setGroupOn-int-) | Bir grup tanımında kriter olarak kullanılan bir alan için gruplama türünü ayarlar. |
| [setPattern(int value)](#setPattern-int-) | Bir grup tanımında kriter olarak kullanılan bir alanın hücre desenini ayarlar. |
| [setStartAt(Object value)](#setStartAt-java.lang.Object-) | Bir grup tanımında kriter olarak kullanılan bir alanın aralık başlangıcını ayarlar. |
### GroupCriterion() {#GroupCriterion--}
```
public GroupCriterion()
```


### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | Bu örnek ile karşılaştırılacak nesne. |

**Returns:**
boolean - **True** ise o, bu örnekle aynı UID değerine sahip bir GroupCriterion'dir; aksi takdirde **false**.
### getAscending() {#getAscending--}
```
public final boolean getAscending()
```


Bir grup tanımında kriter olarak kullanılan bir alanın artan sırada sıralanıp sıralanmadığını gösteren bir değeri alır. Alan azalan sırada sıralanmışsa False.

**Returns:**
boolean - bir grup tanımında kriter olarak kullanılan bir alanın artan sırada sıralanıp sıralanmadığını gösteren bir değer.
### getCellColor() {#getCellColor--}
```
public final Color getCellColor()
```


Bir grup tanımında kriter olarak kullanılan bir alanın hücre arka plan rengini alır.

**Returns:**
java.awt.Color - bir grup tanımında kriter olarak kullanılan bir alanın hücre arka plan rengidir.
### getField() {#getField--}
```
public final int getField()
```


Gruplandırılan alanı alır.

**Returns:**
int - gruplandırılan alan.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


Bir grup tanımındaki kriter için yazı tipini alır.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font for a criterion in a group definition.
### getFontColor() {#getFontColor--}
```
public final Color getFontColor()
```


Bir grup tanımında kriter olarak kullanılan bir alanın yazı tipi rengini alır.

**Returns:**
java.awt.Color - bir grup tanımında kriter olarak kullanılan bir alanın yazı tipi rengidir.
### getGroupInterval() {#getGroupInterval--}
```
public final Object getGroupInterval()
```


Bir grup tanımında kriter olarak kullanılan bir alanın aralığını alır.

**Returns:**
java.lang.Object - bir grup tanımında kriter olarak kullanılan bir alanın aralığı.
### getGroupOn() {#getGroupOn--}
```
public final int getGroupOn()
```


Bir grup tanımında kriter olarak kullanılan bir alanın grup türünü alır.

**Returns:**
int - bir grup tanımında kriter olarak kullanılan bir alanın gruplama türü.
### getPattern() {#getPattern--}
```
public final int getPattern()
```


Bir grup tanımında kriter olarak kullanılan bir alanın hücre desenini alır.

**Returns:**
int - bir grup tanımında kriter olarak kullanılan bir alanın hücre deseni.
### getStartAt() {#getStartAt--}
```
public final Object getStartAt()
```


Bir grup tanımında kriter olarak kullanılan bir alanın aralık başlangıcını alır.

**Returns:**
java.lang.Object - bir grup tanımında kriter olarak kullanılan bir alanın aralık başlangıcı.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Belirli bir tip için bir karma işlevi olarak hizmet eder.

**Returns:**
int - geçerli Nesne için bir karma kodu.
### setAscending(boolean value) {#setAscending-boolean-}
```
public final void setAscending(boolean value)
```


Bir grup tanımında kriter olarak kullanılan bir alanın artan sırada sıralanıp sıralanmadığını gösteren bir değeri ayarlar. Alan azalan sırada sıralanmışsa False.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Bir grup tanımında kriter olarak kullanılan bir alanın artan sırada sıralanıp sıralanmadığını gösteren bir değer. |

### setCellColor(Color value) {#setCellColor-java.awt.Color-}
```
public final void setCellColor(Color value)
```


Bir grup tanımında kriter olarak kullanılan bir alanın hücre arka plan rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.Color | Bir grup tanımında kriter olarak kullanılan bir alanın hücre arka plan rengi. |

### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Gruplandırılan alanı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Gruplandırılan alan. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


Bir grup tanımında kriter için yazı tipini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | bir grup tanımındaki ölçüt için yazı tipi. |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public final void setFontColor(Color value)
```


Bir grup tanımında kriter olarak kullanılan bir alanın yazı tipi rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.Color | bir grup tanımında ölçüt olarak kullanılan alanın yazı tipi rengi. |

### setGroupInterval(Object value) {#setGroupInterval-java.lang.Object-}
```
public final void setGroupInterval(Object value)
```


Bir grup tanımında kriter olarak kullanılan bir alan için aralığı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object | bir grup tanımında ölçüt olarak kullanılan alan için aralık. |

### setGroupOn(int value) {#setGroupOn-int-}
```
public final void setGroupOn(int value)
```


Bir grup tanımında kriter olarak kullanılan bir alan için gruplama türünü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | bir grup tanımında ölçüt olarak kullanılan alan için gruplama türü. |

### setPattern(int value) {#setPattern-int-}
```
public final void setPattern(int value)
```


Bir grup tanımında kriter olarak kullanılan bir alanın hücre desenini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | bir grup tanımında ölçüt olarak kullanılan alan için hücre deseni. |

### setStartAt(Object value) {#setStartAt-java.lang.Object-}
```
public final void setStartAt(Object value)
```


Bir grup tanımında kriter olarak kullanılan bir alanın aralık başlangıcını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object | bir grup tanımında ölçüt olarak kullanılan alan için aralıkların başlangıcı. |

