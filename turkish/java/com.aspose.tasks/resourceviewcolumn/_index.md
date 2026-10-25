---
title: "ResourceViewColumn"
second_title: "Aspose.Tasks for Java API Referansı"
description: "ResourceUsage görünümü ve ResourceSheet görünümünde kullanılan Projects view sınıfı."
type: docs
weight: 261
url: /tr/java/com.aspose.tasks/resourceviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class ResourceViewColumn extends ViewColumn
```

ResourceUsage görünümü ve ResourceSheet görünümünde kullanılan projenin görünüm sınıfı.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-) | Yeni bir [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) sınıfı örneği başlatır. |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-) | Yeni bir [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) sınıfı örneği başlatır. |
| [ResourceViewColumn(int width, int field)](#ResourceViewColumn-int-int-) | Yeni bir [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getColumnText(Resource resource)](#getColumnText-com.aspose.tasks.Resource-) | Geçerli kaynağı sütun metnine dönüştürür. |
| [getField()](#getField--) | Sütun alanını döndürür. |
| [setField(int value)](#setField-int-) | Sütun alanını ayarlar. |
### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)
```


Yeni bir [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String | Sütunun adı. |
| width | int | Sütunun piksel cinsinden genişliği. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Kaynak verisini sütun metnine dönüştüren dönüştürücü. |
| alan | int | Sütun alanı. |

### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)
```


Yeni bir [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String | Sütunun adı. |
| width | int | Sütunun piksel cinsinden genişliği. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Kaynak verisini sütun metnine dönüştüren dönüştürücü. |

### ResourceViewColumn(int width, int field) {#ResourceViewColumn-int-int-}
```
public ResourceViewColumn(int width, int field)
```


Yeni bir [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| width | int | Piksel cinsinden sütun genişliği. |
| alan | int | Sütun alanı. |

### getColumnText(Resource resource) {#getColumnText-com.aspose.tasks.Resource-}
```
public final String getColumnText(Resource resource)
```


Geçerli kaynağı sütun metnine dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| resource | [Resource](../../com.aspose.tasks/resource) | Mevcut kaynak. |

**Returns:**
java.lang.String - Sütun metni.
### getField() {#getField--}
```
public int getField()
```


Sütun alanını döndürür. `Field`.

**Returns:**
int - sütun alanı değeri.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Sütun alanını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | sütun alanı değeri. |

