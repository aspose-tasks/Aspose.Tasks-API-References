---
title: "GanttChartView"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili tampilan GanttChart."
type: docs
weight: 112
url: /id/java/com.aspose.tasks/ganttchartview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public class GanttChartView extends View implements ITimescaledView
```

Mewakili tampilan GanttChart.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [GanttChartView()](#GanttChartView--) | Menginisialisasi instance baru dari kelas [GanttChartView](../../com.aspose.tasks/ganttchartview). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getAutoFilters()](#getAutoFilters--) | Mendapatkan daftar filter otomatis dari tampilan Gantt Chart. |
| [getBarRounding()](#getBarRounding--) | Mendapatkan nilai yang menunjukkan apakah batang dibulatkan ke hari terdekat. |
| [getBarSize()](#getBarSize--) | Mendapatkan tinggi, dalam poin, dari batang Gantt dalam Gantt Chart. |
| [getBarStyles()](#getBarStyles--) | Mendapatkan daftar gaya batang induk (umum) dari tampilan Gantt Chart. |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | Mendapatkan pengaturan tingkat skala waktu bawah tampilan. |
| [getCustomBarStyles()](#getCustomBarStyles--) | Mendapatkan daftar gaya batang khusus yang spesifik untuk tugas dari tampilan Gantt Chart. |
| [getGridlines()](#getGridlines--) | Mendapatkan daftar `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) dari tampilan Gantt Chart. |
| [getHideRollupBarsWhenSummaryExpanded()](#getHideRollupBarsWhenSummaryExpanded--) | Mendapatkan nilai yang menunjukkan apakah batang rollup akan disembunyikan saat memperluas tugas ringkasan. |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | Mendapatkan pengaturan tingkat skala waktu tengah tampilan. |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Mendapatkan warna waktu non-kerja. |
| [getProgressLines()](#getProgressLines--) | Mendapatkan garis kemajuan untuk tampilan Gantt Chart. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Mendapatkan nilai yang menunjukkan apakah batang pada Gantt Chart harus digulung. |
| [getShowBarSplits()](#getShowBarSplits--) | Mendapatkan nilai yang menunjukkan apakah pemisahan tugas pada Gantt Chart harus ditampilkan. |
| [getShowDrawings()](#getShowDrawings--) | Mendapatkan nilai yang menunjukkan apakah gambar pada Gantt Chart harus ditampilkan. |
| [getTableTextStyles()](#getTableTextStyles--) | Mendapatkan daftar gaya teks tabel dari tampilan Gantt Chart. |
| [getTextStyles()](#getTextStyles--) | Mendapatkan daftar [TextStyle](../../com.aspose.tasks/textstyle) dari tampilan Gantt Chart. |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \{@inheritDoc\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | Mendapatkan pengaturan tingkat skala waktu atas tampilan. |
| [setBarRounding(boolean value)](#setBarRounding-boolean-) | Mengatur nilai yang menunjukkan apakah batang dibulatkan ke hari terdekat. |
| [setBarSize(int value)](#setBarSize-int-) | Mengatur tinggi, dalam poin, dari batang Gantt dalam Gantt Chart. |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | Mengatur pengaturan tingkat skala waktu bawah tampilan. |
| [setGridlines(List&lt;Gridlines&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridlines--) | Mengatur daftar `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) dari tampilan Gantt Chart. |
| [setHideRollupBarsWhenSummaryExpanded(boolean value)](#setHideRollupBarsWhenSummaryExpanded-boolean-) | Mengatur nilai yang menunjukkan apakah bar rollup akan disembunyikan saat memperluas tugas rangkuman. |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | Mengatur pengaturan tingkat skala waktu tengah tampilan. |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Mengatur warna waktu non-kerja. |
| [setProgressLines(ProgressLines value)](#setProgressLines-com.aspose.tasks.ProgressLines-) | Mengatur garis kemajuan untuk tampilan Gantt Chart. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Mengatur nilai yang menunjukkan apakah bar pada Gantt Chart harus digulung. |
| [setShowBarSplits(boolean value)](#setShowBarSplits-boolean-) | Mengatur nilai yang menunjukkan apakah pemisahan tugas pada Gantt Chart harus ditampilkan. |
| [setShowDrawings(boolean value)](#setShowDrawings-boolean-) | Mengatur nilai yang menunjukkan apakah gambar pada Gantt Chart harus ditampilkan. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Mengatur daftar [TextStyle](../../com.aspose.tasks/textstyle) dari tampilan Gantt Chart. |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \{@inheritDoc\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | Mengatur pengaturan tingkat skala waktu atas tampilan. |
### GanttChartView() {#GanttChartView--}
```
public GanttChartView()
```


Menginisialisasi instance baru dari kelas [GanttChartView](../../com.aspose.tasks/ganttchartview).

### getAutoFilters() {#getAutoFilters--}
```
public final FilterCollection getAutoFilters()
```


Mendapatkan daftar filter otomatis dari tampilan Gantt Chart.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - a list of auto filters of a Gantt Chart view.
### getBarRounding() {#getBarRounding--}
```
public final boolean getBarRounding()
```


Mendapatkan nilai yang menunjukkan apakah bar dibulatkan ke hari terdekat. Nilai default adalah True.

**Returns:**
boolean - nilai yang menunjukkan apakah bar dibulatkan ke hari terdekat.
### getBarSize() {#getBarSize--}
```
public final int getBarSize()
```


Mendapatkan tinggi, dalam poin, dari batang Gantt dalam Gantt Chart.

**Returns:**
int - tinggi, dalam poin, dari bar Gantt dalam Gantt Chart.
### getBarStyles() {#getBarStyles--}
```
public final List<GanttBarStyle> getBarStyles()
```


Mendapatkan daftar gaya bar induk (umum) dari tampilan Gantt Chart. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - daftar gaya bar induk (umum) dari tampilan Gantt Chart.
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


Mendapatkan pengaturan tingkat skala waktu bawah tampilan. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getCustomBarStyles() {#getCustomBarStyles--}
```
public final List<GanttBarStyle> getCustomBarStyles()
```


Mendapatkan daftar gaya bar khusus per tugas dari tampilan Gantt Chart. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - daftar gaya bar khusus per tugas dari tampilan Gantt Chart.
### getGridlines() {#getGridlines--}
```
public final List<Gridlines> getGridlines()
```


Mendapatkan daftar `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) dari tampilan Gantt Chart.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridlines&gt; - daftar `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) dari tampilan Gantt Chart.
### getHideRollupBarsWhenSummaryExpanded() {#getHideRollupBarsWhenSummaryExpanded--}
```
public final boolean getHideRollupBarsWhenSummaryExpanded()
```


Mendapatkan nilai yang menunjukkan apakah batang rollup akan disembunyikan saat memperluas tugas ringkasan.

**Returns:**
boolean - nilai yang menunjukkan apakah bar rollup akan disembunyikan saat memperluas tugas rangkuman.
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


Mendapatkan pengaturan tingkat skala waktu tengah tampilan. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Mendapatkan warna waktu non-kerja.

**Returns:**
java.awt.Color - warna waktu non-kerja.
### getProgressLines() {#getProgressLines--}
```
public final ProgressLines getProgressLines()
```


Mendapatkan garis kemajuan untuk tampilan Gantt Chart. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Returns:**
[ProgressLines](../../com.aspose.tasks/progresslines) - progress lines for the Gantt Chart view.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Mendapatkan nilai yang menunjukkan apakah batang pada Gantt Chart harus digulung.

**Returns:**
boolean - nilai yang menunjukkan apakah bar pada Gantt Chart harus digulung.
### getShowBarSplits() {#getShowBarSplits--}
```
public final boolean getShowBarSplits()
```


Mendapatkan nilai yang menunjukkan apakah pemisahan tugas pada Gantt Chart harus ditampilkan.

**Returns:**
boolean - nilai yang menunjukkan apakah pemisahan tugas pada Gantt Chart harus ditampilkan.
### getShowDrawings() {#getShowDrawings--}
```
public final boolean getShowDrawings()
```


Mendapatkan nilai yang menunjukkan apakah gambar pada Gantt Chart harus ditampilkan.

**Returns:**
boolean - nilai yang menunjukkan apakah gambar pada Gantt Chart harus ditampilkan.
### getTableTextStyles() {#getTableTextStyles--}
```
public final List<TableTextStyle> getTableTextStyles()
```


Mendapatkan daftar gaya teks tabel dari tampilan Gantt Chart. [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.TableTextStyle&gt; - daftar gaya teks tabel dari tampilan Gantt Chart.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Mendapatkan daftar [TextStyle](../../com.aspose.tasks/textstyle) dari tampilan Gantt Chart.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - daftar [TextStyle](../../com.aspose.tasks/textstyle) dari tampilan Gantt Chart.
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


Mendapatkan persentase untuk mengurangi atau memperbesar jarak antar unit pada tingkat skala waktu.

**Returns:**
int - \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


Mendapatkan pengaturan tingkat skala waktu atas tampilan. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setBarRounding(boolean value) {#setBarRounding-boolean-}
```
public final void setBarRounding(boolean value)
```


Mengatur nilai yang menunjukkan apakah bar dibulatkan ke hari terdekat. Nilai default adalah True.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah bar dibulatkan ke hari terdekat. |

### setBarSize(int value) {#setBarSize-int-}
```
public final void setBarSize(int value)
```


Mengatur tinggi, dalam poin, dari batang Gantt dalam Gantt Chart.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | tinggi, dalam poin, dari bar Gantt dalam Gantt Chart. |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


Mengatur pengaturan tingkat skala waktu bawah tampilan. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | pengaturan tingkat skala waktu bawah tampilan. |

### setGridlines(List&lt;Gridlines&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridlines--}
```
public final void setGridlines(List<Gridlines> value)
```


Mengatur daftar `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) dari tampilan Gantt Chart.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridlines&gt; | daftar `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) dari tampilan Gantt Chart. |

### setHideRollupBarsWhenSummaryExpanded(boolean value) {#setHideRollupBarsWhenSummaryExpanded-boolean-}
```
public final void setHideRollupBarsWhenSummaryExpanded(boolean value)
```


Mengatur nilai yang menunjukkan apakah bar rollup akan disembunyikan saat memperluas tugas rangkuman.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah bar rollup akan disembunyikan saat memperluas tugas rangkuman. |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


Mengatur pengaturan tingkat skala waktu tengah tampilan. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | pengaturan tingkat skala waktu tengah tampilan. |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Mengatur warna waktu non-kerja.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.awt.Color | warna waktu non-kerja. |

### setProgressLines(ProgressLines value) {#setProgressLines-com.aspose.tasks.ProgressLines-}
```
public final void setProgressLines(ProgressLines value)
```


Mengatur garis kemajuan untuk tampilan Gantt Chart. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [ProgressLines](../../com.aspose.tasks/progresslines) | garis kemajuan untuk tampilan Gantt Chart. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Mengatur nilai yang menunjukkan apakah bar pada Gantt Chart harus digulung.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah bar pada Gantt Chart harus digulung. |

### setShowBarSplits(boolean value) {#setShowBarSplits-boolean-}
```
public final void setShowBarSplits(boolean value)
```


Mengatur nilai yang menunjukkan apakah pemisahan tugas pada Gantt Chart harus ditampilkan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah pemisahan tugas pada Gantt Chart harus ditampilkan. |

### setShowDrawings(boolean value) {#setShowDrawings-boolean-}
```
public final void setShowDrawings(boolean value)
```


Mengatur nilai yang menunjukkan apakah gambar pada Gantt Chart harus ditampilkan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah gambar pada Gantt Chart harus ditampilkan. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Mengatur daftar [TextStyle](../../com.aspose.tasks/textstyle) dari tampilan Gantt Chart.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | daftar [TextStyle](../../com.aspose.tasks/textstyle) dari tampilan Gantt Chart. |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


Mengatur persentase untuk mengurangi atau memperbesar jarak antar unit pada tingkat skala waktu.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | \{@inheritDoc\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


Mengatur pengaturan tingkat skala waktu atas tampilan. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | pengaturan tingkat skala waktu atas tampilan. |

