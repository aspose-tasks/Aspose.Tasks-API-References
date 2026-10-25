---
title: "GanttChartView"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir GanttChart görünümünü temsil eder."
type: docs
weight: 112
url: /tr/java/com.aspose.tasks/ganttchartview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public class GanttChartView extends View implements ITimescaledView
```

Bir GanttChart görünümünü temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GanttChartView()](#GanttChartView--) | Yeni bir [GanttChartView](../../com.aspose.tasks/ganttchartview) sınıfının örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getAutoFilters()](#getAutoFilters--) | Bir Gantt Chart görünümünün otomatik filtreler listesini alır. |
| [getBarRounding()](#getBarRounding--) | Çubukların en yakın güne yuvarlanıp yuvarlanmadığını gösteren bir değeri alır. |
| [getBarSize()](#getBarSize--) | Gantt Chart'taki Gantt çubuklarının yüksekliğini (puan cinsinden) alır. |
| [getBarStyles()](#getBarStyles--) | Gantt Chart görünümünün üst (ortak) çubuk stilleri listesini alır. |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | Görünümün alt zaman ölçeği katmanının ayarlarını alır. |
| [getCustomBarStyles()](#getCustomBarStyles--) | Gantt Chart görünümünün özel görev‑özel çubuk stilleri listesini alır. |
| [getGridlines()](#getGridlines--) | Gantt Chart görünümünün `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) listesini alır. |
| [getHideRollupBarsWhenSummaryExpanded()](#getHideRollupBarsWhenSummaryExpanded--) | Özet görevi genişletirken toplama çubuklarının gizlenip gizlenmeyeceğini gösteren bir değeri alır. |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | Görünümün orta zaman ölçeği katmanının ayarlarını alır. |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Çalışma dışı zaman rengini alır. |
| [getProgressLines()](#getProgressLines--) | Gantt Chart görünümü için ilerleme çizgilerini alır. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Gantt Chart'taki çubukların toplanması gerekip gerekmediğini gösteren bir değeri alır. |
| [getShowBarSplits()](#getShowBarSplits--) | Gantt Chart'taki görev bölünmelerinin gösterilip gösterilmeyeceğini belirten bir değeri alır. |
| [getShowDrawings()](#getShowDrawings--) | Gantt Chart'taki çizimlerin gösterilip gösterilmeyeceğini belirten bir değeri alır. |
| [getTableTextStyles()](#getTableTextStyles--) | Gantt Chart görünümünün tablo metin stilleri listesini alır. |
| [getTextStyles()](#getTextStyles--) | Gantt Chart görünümünün [TextStyle](../../com.aspose.tasks/textstyle) listesini alır. |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \{@inheritDoc\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | Görünümün üst zaman ölçeği katmanının ayarlarını alır. |
| [setBarRounding(boolean value)](#setBarRounding-boolean-) | Çubukların en yakın güne yuvarlanıp yuvarlanmayacağını gösteren bir değeri ayarlar. |
| [setBarSize(int value)](#setBarSize-int-) | Gantt Chart'taki Gantt çubuklarının yüksekliğini (puan cinsinden) ayarlar. |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | Görünümün alt zaman ölçeği katmanının ayarlarını ayarlar. |
| [setGridlines(List&lt;Gridlines&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridlines--) | Gantt Chart görünümü için `Gridlines`([getGridlines()](../../com.aspose/tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose/tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) listesini ayarlar. |
| [setHideRollupBarsWhenSummaryExpanded(boolean value)](#setHideRollupBarsWhenSummaryExpanded-boolean-) | Özet görevi genişletirken rollup bars'ın gizleneceğini gösteren bir değeri ayarlar. |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | Görünümün orta zaman ölçeği katmanının ayarlarını belirler. |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Çalışma dışı zaman rengini ayarlar. |
| [setProgressLines(ProgressLines value)](#setProgressLines-com.aspose.tasks.ProgressLines-) | Gantt Chart görünümü için ilerleme çizgilerini ayarlar. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Gantt Chart üzerindeki çubukların toplanması gerekip gerekmediğini gösteren bir değeri ayarlar. |
| [setShowBarSplits(boolean value)](#setShowBarSplits-boolean-) | Gantt Chart üzerindeki görev bölünmelerinin gösterilip gösterilmeyeceğini belirten bir değeri ayarlar. |
| [setShowDrawings(boolean value)](#setShowDrawings-boolean-) | Gantt Chart üzerindeki çizimlerin gösterilip gösterilmeyeceğini belirten bir değeri ayarlar. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Gantt Chart görünümü için [TextStyle](../../com.aspose/tasks/textstyle) listesini ayarlar. |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \{@inheritDoc\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | Görünümün üst zaman ölçeği katmanının ayarlarını belirler. |
### GanttChartView() {#GanttChartView--}
```
public GanttChartView()
```


Yeni bir [GanttChartView](../../com.aspose.tasks/ganttchartview) sınıfının örneğini başlatır.

### getAutoFilters() {#getAutoFilters--}
```
public final FilterCollection getAutoFilters()
```


Bir Gantt Chart görünümünün otomatik filtreler listesini alır.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - a list of auto filters of a Gantt Chart view.
### getBarRounding() {#getBarRounding--}
```
public final boolean getBarRounding()
```


Çubukların en yakın güne yuvarlanıp yuvarlanmayacağını gösteren bir değeri alır. Varsayılan değer True'dur.

**Returns:**
boolean - çubukların en yakın güne yuvarlanıp yuvarlanmayacağını gösteren bir değer.
### getBarSize() {#getBarSize--}
```
public final int getBarSize()
```


Gantt Chart'taki Gantt çubuklarının yüksekliğini (puan cinsinden) alır.

**Returns:**
int - Gantt Chart'taki Gantt çubuklarının yüksekliği (puan cinsinden).
### getBarStyles() {#getBarStyles--}
```
public final List<GanttBarStyle> getBarStyles()
```


Gantt Chart görünümü için ebeveyn (ortak) çubuk stillerinin listesini alır. [GanttBarStyle](../../com.aspose/tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - Gantt Chart görünümü için ebeveyn (ortak) çubuk stillerinin listesi.
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


Görünümün alt zaman ölçeği katmanının ayarlarını alır. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getCustomBarStyles() {#getCustomBarStyles--}
```
public final List<GanttBarStyle> getCustomBarStyles()
```


Gantt Chart görünümü için özel görev‑özel çubuk stillerinin listesini alır. [GanttBarStyle](../../com.aspose/tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - Gantt Chart görünümü için özel görev‑özel çubuk stillerinin listesi.
### getGridlines() {#getGridlines--}
```
public final List<Gridlines> getGridlines()
```


Gantt Chart görünümünün `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) listesini alır.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridlines&gt; - Gantt Chart görünümü için `Gridlines`([getGridlines()](../../com.aspose/tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose/tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) listesidir.
### getHideRollupBarsWhenSummaryExpanded() {#getHideRollupBarsWhenSummaryExpanded--}
```
public final boolean getHideRollupBarsWhenSummaryExpanded()
```


Özet görevi genişletirken toplama çubuklarının gizlenip gizlenmeyeceğini gösteren bir değeri alır.

**Returns:**
boolean - özet görevi genişletirken rollup bars'ın gizleneceğini gösteren bir değer.
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


Görünümün orta zaman ölçeği katmanının ayarlarını alır. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Çalışma dışı zaman rengini alır.

**Returns:**
java.awt.Color - çalışma dışı zaman rengi.
### getProgressLines() {#getProgressLines--}
```
public final ProgressLines getProgressLines()
```


Gantt Chart görünümü için ilerleme çizgilerini alır. `ProgressLines`([getProgressLines()](../../com.aspose/tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose/tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Returns:**
[ProgressLines](../../com.aspose.tasks/progresslines) - progress lines for the Gantt Chart view.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Gantt Chart'taki çubukların toplanması gerekip gerekmediğini gösteren bir değeri alır.

**Returns:**
boolean - Gantt Chart üzerindeki çubukların toplanması gerekip gerekmediğini gösteren bir değer.
### getShowBarSplits() {#getShowBarSplits--}
```
public final boolean getShowBarSplits()
```


Gantt Chart'taki görev bölünmelerinin gösterilip gösterilmeyeceğini belirten bir değeri alır.

**Returns:**
boolean - Gantt Chart üzerindeki görev bölünmelerinin gösterilip gösterilmeyeceğini belirten bir değer.
### getShowDrawings() {#getShowDrawings--}
```
public final boolean getShowDrawings()
```


Gantt Chart'taki çizimlerin gösterilip gösterilmeyeceğini belirten bir değeri alır.

**Returns:**
boolean - Gantt Chart üzerindeki çizimlerin gösterilip gösterilmeyeceğini belirten bir değer.
### getTableTextStyles() {#getTableTextStyles--}
```
public final List<TableTextStyle> getTableTextStyles()
```


Gantt Chart görünümü için tablo metin stillerinin listesini alır. [TableTextStyle](../../com.aspose/tasks/tabletextstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.TableTextStyle&gt; - Gantt Chart görünümü için tablo metin stillerinin listesi.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Gantt Chart görünümünün [TextStyle](../../com.aspose.tasks/textstyle) listesini alır.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - Gantt Chart görünümü için [TextStyle](../../com.aspose/tasks/textstyle) listesidir.
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


Zaman ölçeği katmanındaki birimler arasındaki boşluğu azaltmak veya artırmak için bir yüzde alır.

**Returns:**
int - \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


Görünümün üst zaman ölçeği katmanının ayarlarını alır. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setBarRounding(boolean value) {#setBarRounding-boolean-}
```
public final void setBarRounding(boolean value)
```


Çubukların en yakın güne yuvarlanıp yuvarlanmayacağını belirten bir değer ayarlar. Varsayılan değer True'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Çubukların en yakın güne yuvarlanıp yuvarlanmayacağını belirten bir değer. |

### setBarSize(int value) {#setBarSize-int-}
```
public final void setBarSize(int value)
```


Gantt Chart'taki Gantt çubuklarının yüksekliğini (puan cinsinden) ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Gantt Şeması'ndaki Gantt çubuklarının yüksekliği, puan cinsinden. |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


Görünümün alt zaman ölçeği katmanının ayarlarını belirler. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | görünümün alt zaman ölçeği katmanının ayarları. |

### setGridlines(List&lt;Gridlines&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridlines--}
```
public final void setGridlines(List<Gridlines> value)
```


Gantt Chart görünümü için `Gridlines`([getGridlines()](../../com.aspose/tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose/tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) listesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridlines&gt; | Gantt Şeması görünümünün `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) listesi. |

### setHideRollupBarsWhenSummaryExpanded(boolean value) {#setHideRollupBarsWhenSummaryExpanded-boolean-}
```
public final void setHideRollupBarsWhenSummaryExpanded(boolean value)
```


Özet görevi genişletirken rollup bars'ın gizleneceğini gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Özet görevi genişletirken toplama çubuklarının gizlenip gizlenmeyeceğini belirten bir değer. |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


Görünümün orta zaman ölçeği katmanının ayarlarını belirler. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | görünümün orta zaman ölçeği katmanının ayarları. |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Çalışma dışı zaman rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.Color | Çalışma dışı zaman rengi. |

### setProgressLines(ProgressLines value) {#setProgressLines-com.aspose.tasks.ProgressLines-}
```
public final void setProgressLines(ProgressLines value)
```


Gantt Şeması görünümü için ilerleme çizgilerini ayarlar. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ProgressLines](../../com.aspose.tasks/progresslines) | Gantt Şeması görünümü için ilerleme çizgileri. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Gantt Chart üzerindeki çubukların toplanması gerekip gerekmediğini gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Gantt Şeması üzerindeki çubukların toplanıp toplanmayacağını belirten bir değer. |

### setShowBarSplits(boolean value) {#setShowBarSplits-boolean-}
```
public final void setShowBarSplits(boolean value)
```


Gantt Chart üzerindeki görev bölünmelerinin gösterilip gösterilmeyeceğini belirten bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Gantt Şeması üzerindeki görev bölünmelerinin gösterilip gösterilmeyeceğini belirten bir değer. |

### setShowDrawings(boolean value) {#setShowDrawings-boolean-}
```
public final void setShowDrawings(boolean value)
```


Gantt Chart üzerindeki çizimlerin gösterilip gösterilmeyeceğini belirten bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Gantt Şeması üzerindeki çizimlerin gösterilip gösterilmeyeceğini belirten bir değer. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Gantt Chart görünümü için [TextStyle](../../com.aspose/tasks/textstyle) listesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | Gantt Şeması görünümünün [TextStyle](../../com.aspose.tasks/textstyle) listesi. |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


Zaman ölçeği katmanındaki birimler arasındaki boşluğu azaltmak veya artırmak için bir yüzde belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | \{@inheritDoc\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


Görünümün üst zaman ölçeği katmanının ayarlarını belirler. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | görünümün üst zaman ölçeği katmanının ayarları. |

