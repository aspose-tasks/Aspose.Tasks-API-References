---
title: "XlsxOptions"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Proje sayfalarını XLSX'e render ederken ek seçenekleri belirtmeye izin verir."
type: docs
weight: 368
url: /tr/java/com.aspose.tasks/xlsxoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class XlsxOptions extends SimpleSaveOptions
```

Proje sayfalarını XLSX'e render ederken ek seçenekleri belirtmeye izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [XlsxOptions()](#XlsxOptions--) | Projeyi XLSX formatında kaydetmek için kullanılabilecek yeni bir [XlsxOptions](../../com.aspose.tasks/xlsxoptions) sınıf örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | Render edilecek atama görünüm sütunlarının bir listesini alır ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getEncoding()](#getEncoding--) | Oluşturulan XLSX dosyasının kodlamasını alır. |
| [getResourceView()](#getResourceView--) | Render edilecek kaynak görünüm sütunlarının bir listesini alır ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | XLSX formatında kaydetmek için görünüm sütunlarının ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) listesini alır. |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | Render edilecek atama görünüm sütunlarının bir listesini ayarlar ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Oluşturulan XLSX dosyasının kodlamasını ayarlar. |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | Render edilecek kaynak görünüm sütunlarının bir listesini ayarlar ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | XLSX formatında kaydetmek için görünüm sütunlarının ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) listesini ayarlar. |
### XlsxOptions() {#XlsxOptions--}
```
public XlsxOptions()
```


Projeyi XLSX formatında kaydetmek için kullanılabilecek yeni bir [XlsxOptions](../../com.aspose.tasks/xlsxoptions) sınıf örneği başlatır.

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


Render edilecek atama görünüm sütunlarının bir listesini alır ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Oluşturulan XLSX dosyasının kodlamasını alır. Varsayılan değer java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8'dır.

**Returns:**
java.nio.charset.Charset - oluşturulan XLSX dosyasının kodlaması.
### getResourceView() {#getResourceView--}
```
public final ProjectView getResourceView()
```


Render edilecek kaynak görünüm sütunlarının bir listesini alır ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).
### getView() {#getView--}
```
public final ProjectView getView()
```


XLSX formatında kaydetmek için görünüm sütunlarının ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) listesini alır. Ayarlanmamışsa varsayılan sütunlar kaydedilir.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


Render edilecek atama görünüm sütunlarının bir listesini ayarlar ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | Render edilecek atama görünüm sütunlarının bir listesi ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Oluşturulan XLSX dosyasının kodlamasını ayarlar. Varsayılan değer java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.nio.charset.Charset | oluşturulan XLSX dosyasının kodlaması. |

### setResourceView(ProjectView value) {#setResourceView-com.aspose.tasks.ProjectView-}
```
public final void setResourceView(ProjectView value)
```


Render edilecek kaynak görünüm sütunlarının bir listesini ayarlar ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | Render edilecek kaynak görünüm sütunlarının bir listesi ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


XLSX formatında kaydetmek için görünüm sütunlarının ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) listesini ayarlar. Ayarlanmamışsa varsayılan sütunlar kaydedilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | XLSX formatında kaydetmek için görünüm sütunlarının ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) listesi. |

