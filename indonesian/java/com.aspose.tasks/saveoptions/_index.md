---
title: "SaveOptions"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Ini adalah kelas dasar abstrak untuk kelas-kelas yang memungkinkan pengguna menentukan opsi tambahan saat menyimpan proyek ke format tertentu."
type: docs
weight: 274
url: /id/java/com.aspose.tasks/saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public abstract class SaveOptions extends SimpleSaveOptions
```

Ini adalah kelas dasar abstrak untuk kelas-kelas yang memungkinkan pengguna menentukan opsi tambahan saat menyimpan proyek ke format tertentu.

--------------------

Sebuah instance dari kelas turunan apa pun dari kelas SaveOptions diteruskan ke overload Save aliran atau Save string agar pengguna dapat menentukan opsi khusus saat menyimpan dokumen.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getBarStyles()](#getBarStyles--) | Mendapatkan daftar instance dari kelas [BarStyle](../../com.aspose.tasks/barstyle) yang muncul dalam tampilan proyek. |
| [getCustomPageSize()](#getCustomPageSize--) | Mendapatkan ukuran halaman khusus dalam poin (1 poin = 1/72 inci). |
| [getDrawNonWorkingTime()](#getDrawNonWorkingTime--) | Mendapatkan nilai yang menunjukkan apakah waktu non-kerja harus digambar (Nilai default adalah TRUE). |
| [getEndDate()](#getEndDate--) | Mendapatkan tanggal untuk menyelesaikan rendering. |
| [getFitContent()](#getFitContent--) | Mendapatkan nilai yang menunjukkan apakah tinggi baris harus ditingkatkan agar sesuai dengan isinya. |
| [getGridlines()](#getGridlines--) | Mendapatkan daftar [Gridline](../../com.aspose.tasks/gridline) yang muncul dalam tampilan proyek. |
| [getLegendDrawingOptions()](#getLegendDrawingOptions--) | Mendapatkan nilai yang menentukan cara merender legenda. |
| [getLegendItems()](#getLegendItems--) | Mendapatkan array PageLegendItem yang menentukan batang mana yang harus dirender dalam legenda halaman. |
| [getMarkCriticalTasks()](#getMarkCriticalTasks--) | Mendapatkan nilai yang menunjukkan apakah tugas kritis harus ditampilkan dengan warna merah (Nilai default adalah FALSE). |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Mendapatkan warna waktu non-kerja. |
| [getPageCount()](#getPageCount--) | Mendapatkan jumlah halaman proyek. |
| [getPageSize()](#getPageSize--) | Mendapatkan ukuran halaman yang akan dirender (Nilai default adalah PageSize.A4). |
| [getPresentationFormat()](#getPresentationFormat--) | Mendapatkan `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) di mana dokumen akan disimpan. |
| [getRenderToSinglePage()](#getRenderToSinglePage--) | Mendapatkan nilai yang menunjukkan apakah proyek harus dirender ke satu halaman ketika proyek disimpan dalam format grafis. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Mendapatkan nilai yang menunjukkan apakah subtugas pada bar tugas ringkasan harus ditandai. |
| [getStartDate()](#getStartDate--) | Mendapatkan tanggal untuk memulai rendering. |
| [getTaskLinkDrawingCallback()](#getTaskLinkDrawingCallback--) | Mendapatkan callback yang dapat digunakan untuk menyesuaikan beberapa aspek rendering tautan tugas. |
| [getTextStyles()](#getTextStyles--) | Mendapatkan daftar gaya teks yang diterapkan selama rendering tampilan proyek. |
| [getTimescale()](#getTimescale--) | Mendapatkan nilai `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) yang digunakan untuk mengontrol bagaimana skala waktu (jika ada) dirender ketika proyek disimpan ke format grafis. |
| [getTimescaleFitBehavior()](#getTimescaleFitBehavior--) | Mendapatkan perilaku yang menentukan bagaimana menyelaraskan ujung kanan skala waktu dengan ujung halaman. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Mendapatkan nilai yang menunjukkan apakah kuas gradien harus digunakan saat merender Gantt Chart. |
| [getView()](#getView--) | Mendapatkan daftar kolom tampilan yang akan dirender ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [getViewSettings()](#getViewSettings--) | Mendapatkan tampilan (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) untuk dirender. |
| [isPortrait()](#isPortrait--) | Mendapatkan nilai yang menunjukkan apakah orientasi halaman portrait; mengembalikan false jika orientasi halaman landscape. |
| [setBarStyles(List&lt;BarStyle&gt; value)](#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--) | Mengatur daftar instance kelas [BarStyle](../../com.aspose.tasks/barstyle) yang muncul dalam tampilan proyek. |
| [setCustomPageSize(Dimension2D value)](#setCustomPageSize-java.awt.geom.Dimension2D-) | Mengatur ukuran halaman khusus dalam poin (1 poin = 1/72 inci). |
| [setDrawNonWorkingTime(boolean value)](#setDrawNonWorkingTime-boolean-) | Mengatur nilai yang menunjukkan apakah waktu non-kerja harus digambar (Nilai default adalah TRUE). |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Mengatur tanggal untuk menyelesaikan rendering. |
| [setFitContent(boolean value)](#setFitContent-boolean-) | Mengatur nilai yang menunjukkan apakah tinggi baris harus ditingkatkan agar sesuai dengan isinya. |
| [setGridlines(List&lt;Gridline&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridline--) | Mengatur daftar [Gridline](../../com.aspose.tasks/gridline) yang muncul dalam tampilan proyek. |
| [setLegendDrawingOptions(int value)](#setLegendDrawingOptions-int-) | Mengatur nilai yang menentukan bagaimana merender legenda. |
| [setLegendItems(PageLegendItem[] value)](#setLegendItems-com.aspose.tasks.PageLegendItem---) | Mengatur array PageLegendItem yang menentukan batang mana yang harus dirender dalam legenda halaman. |
| [setMarkCriticalTasks(boolean value)](#setMarkCriticalTasks-boolean-) | Mengatur nilai yang menunjukkan apakah tugas kritis harus ditampilkan dengan warna merah (Nilai default adalah FALSE). |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Mengatur warna waktu non-kerja. |
| [setPageSize(int value)](#setPageSize-int-) | Mengatur ukuran halaman yang akan dirender (Nilai default adalah PageSize.A4). |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Mengatur nilai yang menunjukkan apakah orientasi halaman portrait; mengembalikan false jika orientasi halaman landscape. |
| [setPresentationFormat(int value)](#setPresentationFormat-int-) | Mengatur `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) di mana dokumen akan disimpan. |
| [setRenderToSinglePage(boolean value)](#setRenderToSinglePage-boolean-) | Mengatur nilai yang menunjukkan apakah proyek harus dirender ke satu halaman ketika proyek disimpan dalam format grafis. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Mengatur nilai yang menunjukkan apakah subtugas pada bar tugas ringkasan harus ditandai. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Mengatur tanggal untuk memulai rendering dari. |
| [setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)](#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-) | Mengatur callback yang dapat digunakan untuk menyesuaikan beberapa aspek rendering tautan tugas. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Mengatur daftar gaya teks yang diterapkan selama rendering tampilan proyek. |
| [setTimescale(int value)](#setTimescale-int-) | Mengatur nilai `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) yang digunakan untuk mengontrol bagaimana skala waktu (jika ada) dirender ketika proyek disimpan ke format grafis. |
| [setTimescaleFitBehavior(int value)](#setTimescaleFitBehavior-int-) | Mengatur perilaku yang menentukan cara menyelaraskan ujung kanan skala waktu dengan ujung halaman. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Mengatur nilai yang menunjukkan apakah kuas gradien harus digunakan saat merender Gantt Chart. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Mengatur daftar kolom tampilan yang akan dirender ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [setViewSettings(View value)](#setViewSettings-com.aspose.tasks.View-) | Mengatur tampilan (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) untuk dirender. |
### getBarStyles() {#getBarStyles--}
```
public final List<BarStyle> getBarStyles()
```


Mendapatkan daftar instance dari kelas [BarStyle](../../com.aspose.tasks/barstyle) yang muncul dalam tampilan proyek.

**Returns:**
java.util.List&lt;com.aspose.tasks.BarStyle&gt; - daftar instance kelas [BarStyle](../../com.aspose.tasks/barstyle) yang muncul dalam tampilan proyek.
### getCustomPageSize() {#getCustomPageSize--}
```
public final Dimension2D getCustomPageSize()
```


Mendapatkan ukuran halaman khusus dalam poin (1 poin = 1/72 inci).

**Returns:**
java.awt.geom.Dimension2D - ukuran halaman khusus dalam poin (1 poin = 1/72 inci).
### getDrawNonWorkingTime() {#getDrawNonWorkingTime--}
```
public final boolean getDrawNonWorkingTime()
```


Mendapatkan nilai yang menunjukkan apakah waktu non-kerja harus digambar (Nilai default adalah TRUE).

**Returns:**
boolean - nilai yang menunjukkan apakah waktu non-kerja harus digambar (Nilai default adalah TRUE).
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Mendapatkan tanggal untuk menyelesaikan rendering.

**Returns:**
java.util.Date - tanggal untuk menyelesaikan rendering hingga.
### getFitContent() {#getFitContent--}
```
public final boolean getFitContent()
```


Mendapatkan nilai yang menunjukkan apakah tinggi baris harus ditingkatkan agar sesuai dengan isinya.

**Returns:**
boolean - nilai yang menunjukkan apakah tinggi baris harus ditingkatkan agar sesuai dengan isinya.
### getGridlines() {#getGridlines--}
```
public final List<Gridline> getGridlines()
```


Mendapatkan daftar [Gridline](../../com.aspose.tasks/gridline) yang muncul dalam tampilan proyek.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridline&gt; - daftar [Gridline](../../com.aspose.tasks/gridline) yang muncul dalam tampilan proyek.
### getLegendDrawingOptions() {#getLegendDrawingOptions--}
```
public final int getLegendDrawingOptions()
```


Mendapatkan nilai yang menentukan cara merender legenda. Nilai default adalah LegendDrawingOptions.OnEveryPage.

Hanya berlaku ketika tampilan diagram Gantt dirender.

**Returns:**
int - nilai yang menentukan cara merender legenda.
### getLegendItems() {#getLegendItems--}
```
public final PageLegendItem[] getLegendItems()
```


Mendapatkan array PageLegendItem yang menentukan batang mana yang harus dirender dalam legenda halaman. Jika null, item default akan dirender.

Hanya berlaku ketika tampilan diagram Gantt dirender.

**Returns:**
com.aspose.tasks.PageLegendItem[] - array PageLegendItem yang menentukan batang mana yang harus dirender dalam legenda halaman.
### getMarkCriticalTasks() {#getMarkCriticalTasks--}
```
public final boolean getMarkCriticalTasks()
```


Mendapatkan nilai yang menunjukkan apakah tugas kritis harus ditampilkan dengan warna merah (Nilai default adalah FALSE).

**Returns:**
boolean - nilai yang menunjukkan apakah tugas kritis harus ditampilkan dengan warna merah (Nilai default adalah FALSE).
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Mendapatkan warna waktu non-kerja.

**Returns:**
java.awt.Color - warna waktu non-kerja.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Mendapatkan jumlah halaman proyek.

**Returns:**
int - jumlah halaman proyek.
### getPageSize() {#getPageSize--}
```
public final int getPageSize()
```


Mendapatkan ukuran halaman yang akan dirender (Nilai default adalah PageSize.A4).

**Returns:**
int - ukuran halaman yang akan dirender (Nilai default adalah PageSize.A4).
### getPresentationFormat() {#getPresentationFormat--}
```
public final int getPresentationFormat()
```


Mendapatkan `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) di mana dokumen akan disimpan.

**Returns:**
int - `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) di mana dokumen akan disimpan.
### getRenderToSinglePage() {#getRenderToSinglePage--}
```
public final boolean getRenderToSinglePage()
```


Mendapatkan nilai yang menunjukkan apakah proyek harus dirender ke satu halaman ketika proyek disimpan dalam format grafis. Ukuran halaman akan diubah sehingga proyek yang dirender dapat muat dalam satu halaman.

**Returns:**
boolean - nilai yang menunjukkan apakah proyek harus dirender ke satu halaman ketika proyek disimpan dalam format grafis.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Mendapatkan nilai yang menunjukkan apakah subtugas pada bilah tugas ringkasan harus ditandai. Untuk subtugas, bidang Rollup menunjukkan apakah informasi pada bilah Gantt subtugas akan digabungkan ke bilah tugas ringkasan. Untuk tugas ringkasan, bidang Rollup menunjukkan apakah bilah tugas ringkasan menampilkan bilah yang digabungkan. Anda harus mengatur bidang Rollup untuk tugas ringkasan ke Ya agar subtugas apa pun dapat digabungkan ke mereka.

--------------------

Hanya berlaku ketika tampilan diagram Gantt dirender.

**Returns:**
boolean - nilai yang menunjukkan apakah subtugas pada bilah tugas ringkasan harus ditandai.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Mendapatkan tanggal untuk memulai rendering.

**Returns:**
java.util.Date - tanggal untuk memulai rendering.
### getTaskLinkDrawingCallback() {#getTaskLinkDrawingCallback--}
```
public final TaskLinkDrawingCallbackDelegate getTaskLinkDrawingCallback()
```


Mendapatkan callback yang dapat digunakan untuk menyesuaikan beberapa aspek rendering tautan tugas.

Hanya berlaku ketika tampilan diagram Gantt dirender.

**Returns:**
[TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) - a callback that can be used to customize some aspects of task links rendering.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Mendapatkan daftar gaya teks yang diterapkan selama rendering tampilan proyek.

--------------------

Gaya ini menggantikan gaya yang didefinisikan dengan GanttCharView.setTextStyles.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - daftar gaya teks yang diterapkan selama rendering tampilan proyek.
### getTimescale() {#getTimescale--}
```
public final int getTimescale()
```


Mendapatkan nilai `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) yang digunakan untuk mengontrol bagaimana skala waktu (jika ada) dirender ketika proyek disimpan ke format grafis.

**Returns:**
int - nilai `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) yang digunakan untuk mengontrol bagaimana skala waktu (jika ada) dirender ketika proyek disimpan dalam format grafis.
### getTimescaleFitBehavior() {#getTimescaleFitBehavior--}
```
public final int getTimescaleFitBehavior()
```


Mendapatkan perilaku yang menentukan bagaimana menyelaraskan ujung kanan skala waktu dengan ujung halaman.

**Returns:**
int - perilaku yang menentukan bagaimana menyelaraskan ujung kanan skala waktu dengan ujung halaman.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Mendapatkan nilai yang menunjukkan apakah kuas gradien harus digunakan saat merender Gantt Chart.

--------------------

Hanya berlaku ketika tampilan diagram Gantt dirender.

**Returns:**
boolean - nilai yang menunjukkan apakah kuas gradien harus digunakan saat merender Gantt Chart.
### getView() {#getView--}
```
public final ProjectView getView()
```


Mendapatkan daftar kolom tampilan yang akan dirender ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Jika tidak disetel, maka hanya ID tugas, nama tugas, mulai, dan selesai yang dirender. Jika kedua properti View dan `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) disetel, kolom dari View menggantikan kolom dari ViewSettings.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)).
### getViewSettings() {#getViewSettings--}
```
public final View getViewSettings()
```


Mendapatkan tampilan (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) untuk dirender. Anda dapat menggunakan opsi ini untuk secara eksplisit menentukan tampilan mana yang harus disimpan ke format PDF, HTML, atau Image. Jika properti ini disetel, properti [PresentationFormat](../../com.aspose.tasks/presentationformat) diabaikan ketika proyek disimpan. Tampilan harus berasal dari salah satu layar berikut ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Returns:**
[View](../../com.aspose.tasks/view) - a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Mendapatkan nilai yang menunjukkan apakah orientasi halaman portrait; mengembalikan false jika orientasi halaman landscape.

--------------------

Tidak berlaku ketika SaveOptions.getPageSize() == PageSize.DefinedInView. Dalam kasus ini, [PageSettings.isPortrait()](../../com.aspose.tasks/pagesettings\#isPortrait--) digunakan sebagai gantinya. Tidak berlaku ketika [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) disetel.

**Returns:**
boolean - nilai yang menunjukkan apakah orientasi halaman portrait; mengembalikan false jika orientasi halaman landscape.
### setBarStyles(List&lt;BarStyle&gt; value) {#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--}
```
public final void setBarStyles(List<BarStyle> value)
```


Mengatur daftar instance kelas [BarStyle](../../com.aspose.tasks/barstyle) yang muncul dalam tampilan proyek.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.BarStyle&gt; | daftar instance dari kelas [BarStyle](../../com.aspose.tasks/barstyle) yang muncul dalam tampilan proyek. |

### setCustomPageSize(Dimension2D value) {#setCustomPageSize-java.awt.geom.Dimension2D-}
```
public final void setCustomPageSize(Dimension2D value)
```


Mengatur ukuran halaman khusus dalam poin (1 poin = 1/72 inci).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.awt.geom.Dimension2D | ukuran halaman khusus dalam poin (1 poin = 1/72 inci). |

### setDrawNonWorkingTime(boolean value) {#setDrawNonWorkingTime-boolean-}
```
public final void setDrawNonWorkingTime(boolean value)
```


Mengatur nilai yang menunjukkan apakah waktu non-kerja harus digambar (Nilai default adalah TRUE).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah waktu non-kerja harus digambar (Nilai default adalah TRUE). |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Mengatur tanggal untuk menyelesaikan rendering.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | tanggal untuk menyelesaikan rendering. |

### setFitContent(boolean value) {#setFitContent-boolean-}
```
public final void setFitContent(boolean value)
```


Mengatur nilai yang menunjukkan apakah tinggi baris harus ditingkatkan agar sesuai dengan isinya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah tinggi baris harus ditingkatkan agar sesuai dengan kontennya. |

### setGridlines(List&lt;Gridline&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridline--}
```
public final void setGridlines(List<Gridline> value)
```


Mengatur daftar [Gridline](../../com.aspose.tasks/gridline) yang muncul dalam tampilan proyek.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridline&gt; | daftar [Gridline](../../com.aspose.tasks/gridline) yang muncul dalam tampilan proyek. |

### setLegendDrawingOptions(int value) {#setLegendDrawingOptions-int-}
```
public final void setLegendDrawingOptions(int value)
```


Menetapkan nilai yang menentukan cara merender legenda. Nilai default adalah LegendDrawingOptions.OnEveryPage.

Hanya berlaku ketika tampilan diagram Gantt dirender.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nilai yang menentukan cara merender legenda. |

### setLegendItems(PageLegendItem[] value) {#setLegendItems-com.aspose.tasks.PageLegendItem---}
```
public final void setLegendItems(PageLegendItem[] value)
```


Menetapkan array PageLegendItem yang menentukan bilah mana yang harus dirender dalam legenda halaman. Jika null, item default akan dirender.

Hanya berlaku ketika tampilan diagram Gantt dirender.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [PageLegendItem\[\]](../../com.aspose.tasks/pagelegenditem) | array PageLegendItem yang menentukan bilah mana yang harus dirender dalam legenda halaman. |

### setMarkCriticalTasks(boolean value) {#setMarkCriticalTasks-boolean-}
```
public final void setMarkCriticalTasks(boolean value)
```


Mengatur nilai yang menunjukkan apakah tugas kritis harus ditampilkan dengan warna merah (Nilai default adalah FALSE).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah tugas kritis harus ditampilkan dengan warna merah (Nilai default adalah FALSE). |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Mengatur warna waktu non-kerja.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.awt.Color | warna waktu non-kerja. |

### setPageSize(int value) {#setPageSize-int-}
```
public final void setPageSize(int value)
```


Mengatur ukuran halaman yang akan dirender (Nilai default adalah PageSize.A4).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | ukuran halaman yang akan dirender (Nilai default adalah PageSize.A4). |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Mengatur nilai yang menunjukkan apakah orientasi halaman portrait; mengembalikan false jika orientasi halaman landscape.

--------------------

Tidak berlaku ketika SaveOptions.PageSize == Visualization.PageSize.DefinedInView. Dalam kasus ini [PageSettings.setPortrait(boolean)](../../com.aspose/tasks/pagesettings\#setPortrait-boolean-) digunakan sebagai gantinya. Tidak berlaku ketika [getCustomPageSize()](../../com.aspose/tasks/saveoptions\#getCustomPageSize--) diatur.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah orientasi halaman portrait; mengembalikan false jika orientasi halaman landscape. |

### setPresentationFormat(int value) {#setPresentationFormat-int-}
```
public final void setPresentationFormat(int value)
```


Mengatur `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) di mana dokumen akan disimpan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | int | `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) di mana dokumen akan disimpan. |

### setRenderToSinglePage(boolean value) {#setRenderToSinglePage-boolean-}
```
public final void setRenderToSinglePage(boolean value)
```


Menetapkan nilai yang menunjukkan apakah proyek harus dirender ke satu halaman ketika proyek disimpan dalam format grafis. Ukuran halaman akan diubah sehingga proyek yang dirender dapat muat dalam satu halaman.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah proyek harus dirender ke satu halaman ketika proyek disimpan dalam format grafis. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Menetapkan nilai yang menunjukkan apakah subtugas pada bilah tugas ringkasan harus ditandai. Untuk subtugas, bidang Rollup menunjukkan apakah informasi pada bilah Gantt subtugas akan digabungkan ke bilah tugas ringkasan. Untuk tugas ringkasan, bidang Rollup menunjukkan apakah bilah tugas ringkasan menampilkan bilah yang digabungkan. Anda harus mengatur bidang Rollup untuk tugas ringkasan ke Ya agar subtugas apa pun dapat digabungkan ke dalamnya.

--------------------

Hanya berlaku ketika tampilan diagram Gantt dirender.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah subtugas pada bilah tugas ringkasan harus ditandai. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Mengatur tanggal untuk memulai rendering dari.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | tanggal untuk memulai rendering. |

### setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value) {#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-}
```
public final void setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)
```


Mengatur callback yang dapat digunakan untuk menyesuaikan beberapa aspek rendering tautan tugas.

Hanya berlaku ketika tampilan diagram Gantt dirender.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) | callback yang dapat digunakan untuk menyesuaikan beberapa aspek rendering tautan tugas. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Mengatur daftar gaya teks yang diterapkan selama rendering tampilan proyek.

--------------------

Gaya ini menggantikan gaya yang didefinisikan dengan GanttCharView.setTextStyles.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | daftar gaya teks yang diterapkan selama rendering tampilan proyek. |

### setTimescale(int value) {#setTimescale-int-}
```
public final void setTimescale(int value)
```


Mengatur nilai `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) yang digunakan untuk mengontrol bagaimana skala waktu (jika ada) dirender ketika proyek disimpan ke format grafis.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | int | `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) nilai yang digunakan untuk mengontrol bagaimana skala waktu (jika ada) dirender ketika proyek disimpan dalam format grafis. |

### setTimescaleFitBehavior(int value) {#setTimescaleFitBehavior-int-}
```
public final void setTimescaleFitBehavior(int value)
```


Mengatur perilaku yang menentukan cara menyelaraskan ujung kanan skala waktu dengan ujung halaman.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | perilaku yang menentukan cara menyelaraskan ujung kanan skala waktu dengan ujung halaman. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Mengatur nilai yang menunjukkan apakah kuas gradien harus digunakan saat merender Gantt Chart.

--------------------

Hanya berlaku ketika tampilan diagram Gantt dirender.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah kuas gradien harus digunakan saat merender Diagram Gantt. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Menetapkan daftar kolom tampilan yang akan dirender ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Jika tidak diatur, maka hanya ID tugas, nama tugas, mulai, dan selesai yang akan dirender. Jika properti View dan `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) keduanya diatur, kolom dari View akan menggantikan kolom dari ViewSettings.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | daftar kolom tampilan yang akan dirender ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |

### setViewSettings(View value) {#setViewSettings-com.aspose.tasks.View-}
```
public final void setViewSettings(View value)
```


Menetapkan tampilan (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) untuk dirender. Anda dapat menggunakan opsi ini untuk secara eksplisit menentukan tampilan mana yang harus disimpan ke format PDF, HTML, atau Image. Jika properti ini diatur, properti [PresentationFormat](../../com.aspose.tasks/presentationformat) akan diabaikan ketika proyek disimpan. Tampilan harus berasal dari salah satu layar berikut ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | tampilan (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) untuk dirender. |

