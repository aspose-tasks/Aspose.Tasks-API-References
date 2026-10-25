---
title: "TableTextStyle"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Görünüm tablosunda bir metin stilini temsil eder."
type: docs
weight: 288
url: /tr/java/com.aspose.tasks/tabletextstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.TextStyle](../../com.aspose.tasks/textstyle)
```
public class TableTextStyle extends TextStyle
```

Görünüm tablosunda bir metin stilini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [TableTextStyle(int rowUid)](#TableTextStyle-int-) | Yeni bir [TableTextStyle](../../com.aspose.tasks/tabletextstyle) sınıfı örneği başlatır. |
| [TableTextStyle(int rowUid, FontDescriptor font)](#TableTextStyle-int-com.aspose.tasks.FontDescriptor-) | Belirtilen yazı tipiyle yeni bir [TableTextStyle](../../com.aspose.tasks/tabletextstyle) sınıfı örneği başlatır. |
| [TableTextStyle(int rowUid, float fontSize, int fontStyle)](#TableTextStyle-int-float-int-) | Belirtilen yazı tipi boyutu ve yazı tipi stiliyle yeni bir [TableTextStyle](../../com.aspose.tasks/tabletextstyle) sınıfı örneği başlatır. |
| [TableTextStyle(int rowUid, int fontStyle)](#TableTextStyle-int-int-) | Varsayılan yazı tipi ayarları ve belirtilen yazı tipi stiliyle yeni bir [TableTextStyle](../../com.aspose.tasks/tabletextstyle) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getField()](#getField--) | Stilin uygulanacağı bir alan alır. |
| [getItemType()](#getItemType--) | Metin öğesi tipini döndürür. |
| [getRowUid()](#getRowUid--) | Bir satırın benzersiz kimliğini alır. |
| [setField(int value)](#setField-int-) | Stilin uygulanacağı bir alan ayarlar. |
### TableTextStyle(int rowUid) {#TableTextStyle-int-}
```
public TableTextStyle(int rowUid)
```


Yeni bir [TableTextStyle](../../com.aspose.tasks/tabletextstyle) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowUid | int | Belirtilen bir satırın benzersiz kimliği. |

### TableTextStyle(int rowUid, FontDescriptor font) {#TableTextStyle-int-com.aspose.tasks.FontDescriptor-}
```
public TableTextStyle(int rowUid, FontDescriptor font)
```


Belirtilen yazı tipiyle yeni bir [TableTextStyle](../../com.aspose.tasks/tabletextstyle) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowUid | int | Belirtilen bir satırın benzersiz kimliği. |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | Bir metin stilinin dayandığı yazı tipi. |

### TableTextStyle(int rowUid, float fontSize, int fontStyle) {#TableTextStyle-int-float-int-}
```
public TableTextStyle(int rowUid, float fontSize, int fontStyle)
```


Belirtilen yazı tipi boyutu ve yazı tipi stiliyle yeni bir [TableTextStyle](../../com.aspose.tasks/tabletextstyle) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowUid | int | Belirtilen bir satırın benzersiz kimliği. |
| fontSize | float | Bir metin stilinin dayandığı yazı tipinin boyutu. |
| fontStyle | int | Yazı tipi stili. |

### TableTextStyle(int rowUid, int fontStyle) {#TableTextStyle-int-int-}
```
public TableTextStyle(int rowUid, int fontStyle)
```


Varsayılan yazı tipi ayarları ve belirtilen yazı tipi stiliyle yeni bir [TableTextStyle](../../com.aspose.tasks/tabletextstyle) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowUid | int | Belirtilen bir satırın benzersiz kimliği. |
| fontStyle | int | Yazı tipi stili. |

### getField() {#getField--}
```
public final int getField()
```


Stilin uygulanacağı bir alanı alır. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Returns:**
int - stilin uygulanacağı bir alan.
### getItemType() {#getItemType--}
```
public int getItemType()
```


Metin öğesi tipini döndürür.

**Returns:**
int - TextItemType sayısal tür değeri.
### getRowUid() {#getRowUid--}
```
public final int getRowUid()
```


Bir satırın benzersiz kimliğini alır.

--------------------

Stil bir görünümün tüm satırlarına uygulanacaksa -1 döndürür.

**Returns:**
int - bir satırın benzersiz kimliği.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Stilin uygulanacağı bir alanı ayarlar. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | stilin uygulanacağı bir alan. |

