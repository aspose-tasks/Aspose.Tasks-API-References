---
title: "ViewColumn"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir proje görünümündeki bir sütunu temsil eder."
type: docs
weight: 344
url: /tr/java/com.aspose.tasks/viewcolumn/
---

**Inheritance:**
java.lang.Object
```
public abstract class ViewColumn
```

Bir proje görünümündeki bir sütunu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getField()](#getField--) | Sütun alanını alır. |
| [getName()](#getName--) | Sütun adını alır. |
| [getStringAlignment()](#getStringAlignment--) | Metnin hizalamasını alır ( [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) enumarasyonunun değerlerinden biri olabilir). |
| [getTextStyleModificationCallback()](#getTextStyleModificationCallback--) | Sütunun hücrelerinin görünümünü özelleştirmek için kullanılabilecek geri çağırmayı alır. |
| [getWidth()](#getWidth--) | Sütun genişliğini alır. |
| [setField(int value)](#setField-int-) | Sütun alanını ayarlar. |
| [setStringAlignment(int value)](#setStringAlignment-int-) | Metnin hizalamasını ayarlar ( [HorizontalStringAlignment](../../com.aspose/tasks/horizontalstringalignment) enumarasyonunun değerlerinden biri olabilir). |
| [setTextStyleModificationCallback(ITextStyleModificationCallback value)](#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-) | Sütunun hücrelerinin görünümünü özelleştirmek için kullanılabilecek geri çağırmayı ayarlar. |
### getField() {#getField--}
```
public abstract int getField()
```


Sütun alanını alır. `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Returns:**
int - sütun alanı.
### getName() {#getName--}
```
public final String getName()
```


Sütun adını alır.

**Returns:**
java.lang.String - sütun adı.
### getStringAlignment() {#getStringAlignment--}
```
public final int getStringAlignment()
```


Metnin hizalamasını alır ( [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) enumarasyonunun değerlerinden biri olabilir).

**Returns:**
int - metnin hizalaması ( [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) enumarasyonunun değerlerinden biri olabilir).
### getTextStyleModificationCallback() {#getTextStyleModificationCallback--}
```
public final ITextStyleModificationCallback getTextStyleModificationCallback()
```


Sütunun hücrelerinin görünümünü özelleştirmek için kullanılabilecek geri çağırmayı alır.

**Returns:**
[ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) - the callback which can be used to customize the appearance of the column's cells.
### getWidth() {#getWidth--}
```
public final int getWidth()
```


Sütun genişliğini alır.

**Returns:**
int - sütun genişliği.
### setField(int value) {#setField-int-}
```
public abstract void setField(int value)
```


Sütun alanını ayarlar. `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | sütun alanı. |

### setStringAlignment(int value) {#setStringAlignment-int-}
```
public final void setStringAlignment(int value)
```


Metnin hizalamasını ayarlar ( [HorizontalStringAlignment](../../com.aspose/tasks/horizontalstringalignment) enumarasyonunun değerlerinden biri olabilir).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | int | metnin hizalaması ( [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) enumarasyonunun değerlerinden biri olabilir). |

### setTextStyleModificationCallback(ITextStyleModificationCallback value) {#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-}
```
public final void setTextStyleModificationCallback(ITextStyleModificationCallback value)
```


Sütunun hücrelerinin görünümünü özelleştirmek için kullanılabilecek geri çağırmayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) | sütunun hücrelerinin görünümünü özelleştirmek için kullanılabilecek geri çağırma. |

