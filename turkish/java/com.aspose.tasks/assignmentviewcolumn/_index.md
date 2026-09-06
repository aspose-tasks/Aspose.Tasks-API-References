---
title: "AssignmentViewColumn"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Projeler görünüm sınıfı."
type: docs
weight: 19
url: /tr/java/com.aspose.tasks/assignmentviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public class AssignmentViewColumn extends ViewColumn
```

Projenin görünüm sınıfı.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)](#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-) | AssignmentViewColumn sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getColumnText(ResourceAssignment assignment)](#getColumnText-com.aspose.tasks.ResourceAssignment-) | Mevcut kaynak atamasını sütun metnine dönüştürür. |
| [getField()](#getField--) | Sütun alanını döndürür. |
| [setField(int value)](#setField-int-) | Sütun alanını ayarlar. |
### AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter) {#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-}
```
public AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)
```


AssignmentViewColumn sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String | Sütunun adı. |
| width | int | Sütunun piksel cinsinden genişliği. |
| converter | [AssignmentToColumnTextConverter](../../com.aspose.tasks/assignmenttocolumntextconverter) | Atama verisini sütun metnine dönüştürücü. |

### getColumnText(ResourceAssignment assignment) {#getColumnText-com.aspose.tasks.ResourceAssignment-}
```
public String getColumnText(ResourceAssignment assignment)
```


Mevcut kaynak atamasını sütun metnine dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| assignment | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Mevcut atama. |

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

