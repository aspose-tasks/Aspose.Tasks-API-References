---
title: "GanttChartColumn"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Projeler görünüm sınıfı"
type: docs
weight: 111
url: /tr/java/com.aspose.tasks/ganttchartcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class GanttChartColumn extends ViewColumn
```

Proje görünüm sınıfı
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-) | GanttChartColumn sınıfının yeni bir örneğini başlatır. |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-) | GanttChartColumn sınıfının yeni bir örneğini başlatır. |
| [GanttChartColumn(int width, int field)](#GanttChartColumn-int-int-) | GanttChartColumn sınıfının yeni bir örneğini başlatır. |
| [GanttChartColumn(String name, int width, int field)](#GanttChartColumn-java.lang.String-int-int-) | GanttChartColumn sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getColumnText(Task task)](#getColumnText-com.aspose.tasks.Task-) | Geçerli görevi sütun metnine dönüştürür. |
| [getField()](#getField--) | Sütun alanını döndürür. |
| [setField(int value)](#setField-int-) | Sütun alanını ayarlar. |
### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)
```


GanttChartColumn sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String | Sütunun adı. |
| width | int | Sütunun piksel cinsinden genişliği. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Görev verisini sütun metnine dönüştüren dönüştürücü. |
| alan | int | Sütun alanı. |

### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)
```


GanttChartColumn sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String | Sütunun adı. |
| width | int | Sütunun piksel cinsinden genişliği. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Görev verisini sütun metnine dönüştüren dönüştürücü. |

### GanttChartColumn(int width, int field) {#GanttChartColumn-int-int-}
```
public GanttChartColumn(int width, int field)
```


GanttChartColumn sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| width | int | Piksel cinsinden sütun genişliği. |
| alan | int | Sütun alanı. |

### GanttChartColumn(String name, int width, int field) {#GanttChartColumn-java.lang.String-int-int-}
```
public GanttChartColumn(String name, int width, int field)
```


GanttChartColumn sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String | Sütun adı. |
| width | int | Piksel cinsinden sütun genişliği. |
| alan | int | Sütun alanı. |

### getColumnText(Task task) {#getColumnText-com.aspose.tasks.Task-}
```
public final String getColumnText(Task task)
```


Geçerli görevi sütun metnine dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Geçerli görev. |

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

