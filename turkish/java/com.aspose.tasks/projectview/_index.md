---
title: "ProjectView"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Projeler görünüm sınıfı"
type: docs
weight: 228
url: /tr/java/com.aspose.tasks/projectview/
---

**Inheritance:**
java.lang.Object
```
public class ProjectView
```

Proje görünüm sınıfı
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ProjectView(Iterable&lt;ViewColumn&gt; columns)](#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--) | [ProjectView](../../com.aspose.tasks/projectview) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getColumns()](#getColumns--) | Proje görünümü sütunlarını alır. |
| [getDefaultAssignmentView()](#getDefaultAssignmentView--) | Uid, görev adı, kaynak adı, iş ve süre atama sütunlarını içerir. |
| [getDefaultGanttChartView()](#getDefaultGanttChartView--) | id, göstergeler, ad, süre, başlangıç ve bitiş görev sütunlarını içerir. |
| [getDefaultResourceSheetView()](#getDefaultResourceSheetView--) | Uid, kaynak adı, tür, malzeme etiketi, baş harfler, grup, maksimum birimler, standart oran, fazla mesai oranı, kullanım başına maliyet, birikim zamanı, temel takvim ve kod kaynak sütunlarını içerir. |
| [getDefaultResourceUsageView()](#getDefaultResourceUsageView--) | Uid, ad, başlangıç, bitiş ve iş kaynağı sütunlarını içerir. |
| [getDefaultTaskSheetView()](#getDefaultTaskSheetView--) | id, göstergeler, ad, süre, başlangıç, bitiş, öncüller ve kaynak adları görev sütunlarını içerir. |
### ProjectView(Iterable&lt;ViewColumn&gt; columns) {#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--}
```
public ProjectView(Iterable<ViewColumn> columns)
```


[ProjectView](../../com.aspose.tasks/projectview) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütunlar | java.lang.Iterable&lt;com.aspose.tasks.ViewColumn&gt; | Görünüm sütunlarının bir listesi. |

### getColumns() {#getColumns--}
```
public final List<ViewColumn> getColumns()
```


Proje görünümü sütunlarını alır.

**Returns:**
java.util.List&lt;com.aspose.tasks.ViewColumn&gt; - proje görünüm sütunları.
### getDefaultAssignmentView() {#getDefaultAssignmentView--}
```
public static ProjectView getDefaultAssignmentView()
```


Uid, görev adı, kaynak adı, iş ve süre atama sütunlarını içerir.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn).
### getDefaultGanttChartView() {#getDefaultGanttChartView--}
```
public static ProjectView getDefaultGanttChartView()
```


id, göstergeler, ad, süre, başlangıç ve bitiş görev sütunlarını içerir.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
### getDefaultResourceSheetView() {#getDefaultResourceSheetView--}
```
public static ProjectView getDefaultResourceSheetView()
```


Uid, kaynak adı, tür, malzeme etiketi, baş harfler, grup, maksimum birimler, standart oran, fazla mesai oranı, kullanım başına maliyet, birikim zamanı, temel takvim ve kod kaynak sütunlarını içerir.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultResourceUsageView() {#getDefaultResourceUsageView--}
```
public static ProjectView getDefaultResourceUsageView()
```


Uid, ad, başlangıç, bitiş ve iş kaynağı sütunlarını içerir.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultTaskSheetView() {#getDefaultTaskSheetView--}
```
public static ProjectView getDefaultTaskSheetView()
```


id, göstergeler, ad, süre, başlangıç, bitiş, öncüller ve kaynak adları görev sütunlarını içerir.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
