---
title: "XlsxOptions"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mengizinkan penentuan opsi tambahan saat merender halaman proyek ke XLSX."
type: docs
weight: 368
url: /id/java/com.aspose.tasks/xlsxoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class XlsxOptions extends SimpleSaveOptions
```

Mengizinkan penentuan opsi tambahan saat merender halaman proyek ke XLSX.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [XlsxOptions()](#XlsxOptions--) | Menginisialisasi instance baru dari kelas [XlsxOptions](../../com.aspose.tasks/xlsxoptions) yang dapat digunakan untuk menyimpan proyek dalam format XLSX. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | Mendapatkan daftar kolom tampilan penugasan untuk dirender ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getEncoding()](#getEncoding--) | Mendapatkan enkoding file XLSX yang dihasilkan. |
| [getResourceView()](#getResourceView--) | Mendapatkan daftar kolom tampilan sumber daya untuk dirender ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | Mendapatkan daftar kolom tampilan ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) untuk disimpan ke format XLSX. |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | Mengatur daftar kolom tampilan penugasan untuk dirender ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Mengatur enkoding file XLSX yang dihasilkan. |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | Mengatur daftar kolom tampilan sumber daya untuk dirender ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Mengatur daftar kolom tampilan ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) untuk disimpan ke format XLSX. |
### XlsxOptions() {#XlsxOptions--}
```
public XlsxOptions()
```


Menginisialisasi instance baru dari kelas [XlsxOptions](../../com.aspose.tasks/xlsxoptions) yang dapat digunakan untuk menyimpan proyek dalam format XLSX.

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


Mendapatkan daftar kolom tampilan penugasan untuk dirender ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Mendapatkan enkoding file XLSX yang dihasilkan. Nilai defaultnya adalah java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Returns:**
java.nio.charset.Charset - enkoding file XLSX yang dihasilkan.
### getResourceView() {#getResourceView--}
```
public final ProjectView getResourceView()
```


Mendapatkan daftar kolom tampilan sumber daya untuk dirender ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).
### getView() {#getView--}
```
public final ProjectView getView()
```


Mendapatkan daftar kolom tampilan ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) untuk disimpan ke format XLSX. Jika tidak diatur maka kolom default akan disimpan.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


Mengatur daftar kolom tampilan penugasan untuk dirender ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | daftar kolom tampilan penugasan untuk dirender ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Mengatur enkoding file XLSX yang dihasilkan. Nilai defaultnya adalah java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.nio.charset.Charset | enkoding file XLSX yang dihasilkan. |

### setResourceView(ProjectView value) {#setResourceView-com.aspose.tasks.ProjectView-}
```
public final void setResourceView(ProjectView value)
```


Mengatur daftar kolom tampilan sumber daya untuk dirender ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | daftar kolom tampilan sumber daya untuk dirender ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Mengatur daftar kolom tampilan ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) untuk disimpan ke format XLSX. Jika tidak diatur maka kolom default akan disimpan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | daftar kolom tampilan ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) untuk disimpan ke format XLSX. |

