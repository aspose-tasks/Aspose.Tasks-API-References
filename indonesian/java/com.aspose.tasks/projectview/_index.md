---
title: "ProjectView"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Kelas tampilan Projects."
type: docs
weight: 228
url: /id/java/com.aspose.tasks/projectview/
---

**Inheritance:**
java.lang.Object
```
public class ProjectView
```

Kelas tampilan proyek
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ProjectView(Iterable&lt;ViewColumn&gt; columns)](#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--) | Menginisialisasi instance baru dari kelas [ProjectView](../../com.aspose.tasks/projectview). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getColumns()](#getColumns--) | Mendapatkan kolom tampilan proyek. |
| [getDefaultAssignmentView()](#getDefaultAssignmentView--) | Menyertakan kolom Uid, nama tugas, nama sumber daya, pekerjaan, dan durasi penugasan. |
| [getDefaultGanttChartView()](#getDefaultGanttChartView--) | Menyertakan id, indikator, nama, durasi, mulai, dan selesai kolom tugas. |
| [getDefaultResourceSheetView()](#getDefaultResourceSheetView--) | Menyertakan Uid, nama sumber daya, tipe, label material, inisial, grup, unit maksimum, tarif standar, tarif lembur, biaya per penggunaan, akrual pada, kalender dasar, dan kode kolom sumber daya. |
| [getDefaultResourceUsageView()](#getDefaultResourceUsageView--) | Menyertakan Uid, nama, mulai, selesai, dan kolom sumber daya kerja. |
| [getDefaultTaskSheetView()](#getDefaultTaskSheetView--) | Menyertakan id, indikator, nama, durasi, mulai, selesai, pendahulu, dan nama sumber daya kolom tugas. |
### ProjectView(Iterable&lt;ViewColumn&gt; columns) {#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--}
```
public ProjectView(Iterable<ViewColumn> columns)
```


Menginisialisasi instance baru dari kelas [ProjectView](../../com.aspose.tasks/projectview).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| kolom | java.lang.Iterable&lt;com.aspose.tasks.ViewColumn&gt; | Daftar kolom tampilan. |

### getColumns() {#getColumns--}
```
public final List<ViewColumn> getColumns()
```


Mendapatkan kolom tampilan proyek.

**Returns:**
java.util.List&lt;com.aspose.tasks.ViewColumn&gt; - kolom tampilan proyek.
### getDefaultAssignmentView() {#getDefaultAssignmentView--}
```
public static ProjectView getDefaultAssignmentView()
```


Menyertakan kolom Uid, nama tugas, nama sumber daya, pekerjaan, dan durasi penugasan.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn).
### getDefaultGanttChartView() {#getDefaultGanttChartView--}
```
public static ProjectView getDefaultGanttChartView()
```


Menyertakan id, indikator, nama, durasi, mulai, dan selesai kolom tugas.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
### getDefaultResourceSheetView() {#getDefaultResourceSheetView--}
```
public static ProjectView getDefaultResourceSheetView()
```


Menyertakan Uid, nama sumber daya, tipe, label material, inisial, grup, unit maksimum, tarif standar, tarif lembur, biaya per penggunaan, akrual pada, kalender dasar, dan kode kolom sumber daya.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultResourceUsageView() {#getDefaultResourceUsageView--}
```
public static ProjectView getDefaultResourceUsageView()
```


Menyertakan Uid, nama, mulai, selesai, dan kolom sumber daya kerja.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultTaskSheetView() {#getDefaultTaskSheetView--}
```
public static ProjectView getDefaultTaskSheetView()
```


Menyertakan id, indikator, nama, durasi, mulai, selesai, pendahulu, dan nama sumber daya kolom tugas.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
