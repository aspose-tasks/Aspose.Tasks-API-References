---
title: "CsvOptions"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Proje CSV'ye kaydedilirken ek seçeneklerin belirtilmesine izin verir."
type: docs
weight: 56
url: /tr/java/com.aspose.tasks/csvoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class CsvOptions extends SimpleSaveOptions
```

Proje CSV'ye kaydedilirken ek seçeneklerin belirtilmesine izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CsvOptions()](#CsvOptions--) | CSV formatında proje kaydetmek için kullanılabilecek yeni bir [CsvOptions](../../com.aspose/tasks/csvoptions) sınıfının bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getDataCategory()](#getDataCategory--) | Kaydedilecek bir veri kategorisini alır. |
| [getEncoding()](#getEncoding--) | CSV'yi kaydetmek için kullanılan kodlamayı alır. |
| [getIncludeHeaders()](#getIncludeHeaders--) | Başlıkların dahil edilip edilmeyeceğini gösteren değeri alır (varsayılan değer TRUE'dır). |
| [getTextDelimiter()](#getTextDelimiter--) | Metin sınırlayıcısını alır. |
| [getView()](#getView--) | XLSX formatında kaydetmek için görünüm sütunlarının ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) listesini alır. |
| [setDataCategory(int value)](#setDataCategory-int-) | Kaydedilecek bir veri kategorisini ayarlar. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | CSV'yi kaydetmek için bir kodlama ayarlar. |
| [setIncludeHeaders(boolean value)](#setIncludeHeaders-boolean-) | Başlıkların dahil edilip edilmeyeceğini gösteren değeri ayarlar (varsayılan değer TRUE'dır). |
| [setTextDelimiter(int value)](#setTextDelimiter-int-) | Metin sınırlayıcısını ayarlar. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | XLSX formatında kaydetmek için görünüm sütunlarının ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) listesini ayarlar. |
### CsvOptions() {#CsvOptions--}
```
public CsvOptions()
```


CSV formatında proje kaydetmek için kullanılabilecek yeni bir [CsvOptions](../../com.aspose/tasks/csvoptions) sınıfının bir örneğini başlatır.

### getDataCategory() {#getDataCategory--}
```
public final int getDataCategory()
```


Kaydedilecek bir veri kategorisini alır.

**Returns:**
int - kaydedilecek bir veri kategorisi.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


CSV'yi kaydetmek için kullanılan kodlamayı alır.

**Returns:**
java.nio.charset.Charset - CSV'yi kaydetmek için bir kodlama.
### getIncludeHeaders() {#getIncludeHeaders--}
```
public final boolean getIncludeHeaders()
```


Başlıkların dahil edilip edilmeyeceğini gösteren değeri alır (varsayılan değer TRUE'dır).

**Returns:**
boolean - başlıkların dahil edilip edilmeyeceğini gösteren değer (varsayılan değer TRUE'dır).
### getTextDelimiter() {#getTextDelimiter--}
```
public final int getTextDelimiter()
```


Metin sınırlayıcısını alır.

**Returns:**
int - bir metin sınırlayıcı.
### getView() {#getView--}
```
public final ProjectView getView()
```


XLSX formatında kaydetmek için görünüm sütunlarının ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) listesini alır. Ayarlanmamışsa varsayılan sütunlar kaydedilir.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setDataCategory(int value) {#setDataCategory-int-}
```
public final void setDataCategory(int value)
```


Kaydedilecek bir veri kategorisini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | kaydedilecek bir veri kategorisi. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


CSV'yi kaydetmek için bir kodlama ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.nio.charset.Charset | CSV'yi kaydetmek için bir kodlama. |

### setIncludeHeaders(boolean value) {#setIncludeHeaders-boolean-}
```
public final void setIncludeHeaders(boolean value)
```


Başlıkların dahil edilip edilmeyeceğini gösteren değeri ayarlar (varsayılan değer TRUE'dır).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | başlıkların dahil edilip edilmeyeceğini gösteren değer (varsayılan değer TRUE'dır). |

### setTextDelimiter(int value) {#setTextDelimiter-int-}
```
public final void setTextDelimiter(int value)
```


Metin sınırlayıcısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | bir metin sınırlayıcı. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


XLSX formatında kaydetmek için görünüm sütunlarının ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) listesini ayarlar. Ayarlanmamışsa varsayılan sütunlar kaydedilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | XLSX formatında kaydetmek için görünüm sütunlarının ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) listesi. |

