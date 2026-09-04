---
title: "GanttChartView"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل عرض مخطط جانت."
type: docs
weight: 112
url: /ar/java/com.aspose.tasks/ganttchartview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public class GanttChartView extends View implements ITimescaledView
```

يمثل عرض مخطط جانت.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GanttChartView()](#GanttChartView--) | يُنشئ مثيلاً جديدًا لفئة [GanttChartView](../../com.aspose.tasks/ganttchartview). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getAutoFilters()](#getAutoFilters--) | يحصل على قائمة بالمرشحات التلقائية لعرض مخطط جانت. |
| [getBarRounding()](#getBarRounding--) | يحصل على قيمة تشير إلى ما إذا كانت الأشرطة تُقرب إلى أقرب يوم. |
| [getBarSize()](#getBarSize--) | يحصل على الارتفاع، بالنقاط، لأشرطة جانت في مخطط جانت. |
| [getBarStyles()](#getBarStyles--) | يحصل على قائمة بأنماط الأشرطة الأصلية (العامة) لعرض مخطط جانت. |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | يحصل على إعدادات الطبقة السفلية لمقياس الوقت في العرض. |
| [getCustomBarStyles()](#getCustomBarStyles--) | يحصل على قائمة بأنماط الأشرطة المخصصة الخاصة بالمهمة لعرض مخطط جانت. |
| [getGridlines()](#getGridlines--) | يحصل على قائمة بـ `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) لعرض مخطط جانت. |
| [getHideRollupBarsWhenSummaryExpanded()](#getHideRollupBarsWhenSummaryExpanded--) | يحصل على قيمة تشير إلى ما إذا كانت أشرطة التجميع ستُخفى عند توسيع مهمة الملخص. |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | يحصل على إعدادات الطبقة الوسطى لمقياس الوقت في العرض. |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | يحصل على لون وقت غير العمل. |
| [getProgressLines()](#getProgressLines--) | يحصل على خطوط التقدم لعرض مخطط جانت. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | يحصل على قيمة تشير إلى ما إذا كان يجب تجميع الأشرطة في مخطط جانت. |
| [getShowBarSplits()](#getShowBarSplits--) | يحصل على قيمة تشير إلى ما إذا كان يجب إظهار تقسيمات المهام في مخطط جانت. |
| [getShowDrawings()](#getShowDrawings--) | يحصل على قيمة تشير إلى ما إذا كان يجب إظهار الرسومات في مخطط جانت. |
| [getTableTextStyles()](#getTableTextStyles--) | يحصل على قائمة بأنماط نص الجدول لعرض مخطط جانت. |
| [getTextStyles()](#getTextStyles--) | يحصل على قائمة بـ [TextStyle](../../com.aspose.tasks/textstyle) لعرض مخطط جانت. |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \{@inheritDoc\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | يحصل على إعدادات الطبقة العليا لمقياس الوقت في العرض. |
| [setBarRounding(boolean value)](#setBarRounding-boolean-) | يضبط قيمة تشير إلى ما إذا كانت الأشرطة تُقرب إلى أقرب يوم. |
| [setBarSize(int value)](#setBarSize-int-) | يضبط الارتفاع، بالنقاط، لأشرطة جانت في مخطط جانت. |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | يضبط إعدادات الطبقة السفلية لمقياس الوقت في العرض. |
| [setGridlines(List&lt;Gridlines&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridlines--) | يضبط قائمة من `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) لعرض مخطط جانت. |
| [setHideRollupBarsWhenSummaryExpanded(boolean value)](#setHideRollupBarsWhenSummaryExpanded-boolean-) | يضبط قيمة تشير إلى ما إذا كانت أشرطة التجميع ستُخفى عند توسيع مهمة الملخص. |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | يضبط إعدادات مستوى المقياس الزمني الأوسط للعرض. |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | يضبط لون الوقت غير العامل. |
| [setProgressLines(ProgressLines value)](#setProgressLines-com.aspose.tasks.ProgressLines-) | يضبط خطوط التقدم لعرض مخطط جانت. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تجميع الأشرطة في مخطط جانت. |
| [setShowBarSplits(boolean value)](#setShowBarSplits-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب إظهار تقسيمات المهام في مخطط جانت. |
| [setShowDrawings(boolean value)](#setShowDrawings-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب إظهار الرسومات في مخطط جانت. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | يضبط قائمة من [TextStyle](../../com.aspose.tasks/textstyle) لعرض مخطط جانت. |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \{@inheritDoc\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | يضبط إعدادات مستوى المقياس الزمني العلوي للعرض. |
### GanttChartView() {#GanttChartView--}
```
public GanttChartView()
```


يُنشئ مثيلاً جديدًا لفئة [GanttChartView](../../com.aspose.tasks/ganttchartview).

### getAutoFilters() {#getAutoFilters--}
```
public final FilterCollection getAutoFilters()
```


يحصل على قائمة بالمرشحات التلقائية لعرض مخطط جانت.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - a list of auto filters of a Gantt Chart view.
### getBarRounding() {#getBarRounding--}
```
public final boolean getBarRounding()
```


يحصل على قيمة تشير إلى ما إذا كانت الأشرطة تُقرب إلى أقرب يوم. القيمة الافتراضية هي True.

**Returns:**
boolean - قيمة تشير إلى ما إذا كانت الأشرطة تُقرب إلى أقرب يوم.
### getBarSize() {#getBarSize--}
```
public final int getBarSize()
```


يحصل على الارتفاع، بالنقاط، لأشرطة جانت في مخطط جانت.

**Returns:**
int - الارتفاع، بالنقاط، لأشرطة جانت في مخطط جانت.
### getBarStyles() {#getBarStyles--}
```
public final List<GanttBarStyle> getBarStyles()
```


يحصل على قائمة بأنماط الأشرطة الأب (العامة) لعرض مخطط جانت. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - قائمة بأنماط الأشرطة الأب (العامة) لعرض مخطط جانت.
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


يحصل على إعدادات مستوى المقياس الزمني السفلي للعرض. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getCustomBarStyles() {#getCustomBarStyles--}
```
public final List<GanttBarStyle> getCustomBarStyles()
```


يحصل على قائمة بأنماط الأشرطة المخصصة الخاصة بالمهام لعرض مخطط جانت. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - قائمة بأنماط الأشرطة المخصصة الخاصة بالمهام لعرض مخطط جانت.
### getGridlines() {#getGridlines--}
```
public final List<Gridlines> getGridlines()
```


يحصل على قائمة بـ `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) لعرض مخطط جانت.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridlines&gt; - قائمة من `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) لعرض مخطط جانت.
### getHideRollupBarsWhenSummaryExpanded() {#getHideRollupBarsWhenSummaryExpanded--}
```
public final boolean getHideRollupBarsWhenSummaryExpanded()
```


يحصل على قيمة تشير إلى ما إذا كانت أشرطة التجميع ستُخفى عند توسيع مهمة الملخص.

**Returns:**
boolean - قيمة تشير إلى ما إذا كانت أشرطة التجميع ستُخفى عند توسيع مهمة الملخص.
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


يحصل على إعدادات مستوى المقياس الزمني الأوسط للعرض. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


يحصل على لون وقت غير العمل.

**Returns:**
java.awt.Color - لون الوقت غير العامل.
### getProgressLines() {#getProgressLines--}
```
public final ProgressLines getProgressLines()
```


يحصل على خطوط التقدم لعرض مخطط جانت. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Returns:**
[ProgressLines](../../com.aspose.tasks/progresslines) - progress lines for the Gantt Chart view.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


يحصل على قيمة تشير إلى ما إذا كان يجب تجميع الأشرطة في مخطط جانت.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب تجميع الأشرطة في مخطط جانت.
### getShowBarSplits() {#getShowBarSplits--}
```
public final boolean getShowBarSplits()
```


يحصل على قيمة تشير إلى ما إذا كان يجب إظهار تقسيمات المهام في مخطط جانت.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب إظهار تقسيمات المهام في مخطط جانت.
### getShowDrawings() {#getShowDrawings--}
```
public final boolean getShowDrawings()
```


يحصل على قيمة تشير إلى ما إذا كان يجب إظهار الرسومات في مخطط جانت.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب إظهار الرسومات في مخطط جانت.
### getTableTextStyles() {#getTableTextStyles--}
```
public final List<TableTextStyle> getTableTextStyles()
```


يحصل على قائمة بأنماط نص الجدول لعرض مخطط جانت. [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.TableTextStyle&gt; - قائمة بأنماط نص الجدول لعرض مخطط جانت.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


يحصل على قائمة بـ [TextStyle](../../com.aspose.tasks/textstyle) لعرض مخطط جانت.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - قائمة من [TextStyle](../../com.aspose.tasks/textstyle) لعرض مخطط جانت.
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


يحصل على نسبة مئوية لتقليل أو تكبير المسافة بين الوحدات في مستوى المقياس الزمني.

**Returns:**
int - \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


يحصل على إعدادات مستوى المقياس الزمني العلوي للعرض. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setBarRounding(boolean value) {#setBarRounding-boolean-}
```
public final void setBarRounding(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت الأشرطة تُقرب إلى أقرب يوم. القيمة الافتراضية هي True.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كانت الأشرطة تُقرب إلى أقرب يوم. |

### setBarSize(int value) {#setBarSize-int-}
```
public final void setBarSize(int value)
```


يضبط الارتفاع، بالنقاط، لأشرطة جانت في مخطط جانت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | الارتفاع، بالنقاط، لأشرطة Gantt في مخطط Gantt. |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


يضبط إعدادات مستوى المقياس الزمني السفلي للعرض. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | إعدادات مستوى المقياس الزمني السفلي للعرض. |

### setGridlines(List&lt;Gridlines&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridlines--}
```
public final void setGridlines(List<Gridlines> value)
```


يضبط قائمة من `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) لعرض مخطط جانت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridlines&gt; | قائمة من `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) لعرض مخطط Gantt. |

### setHideRollupBarsWhenSummaryExpanded(boolean value) {#setHideRollupBarsWhenSummaryExpanded-boolean-}
```
public final void setHideRollupBarsWhenSummaryExpanded(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت أشرطة التجميع ستُخفى عند توسيع مهمة الملخص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كانت أشرطة التجميع ستُخفى عند توسيع مهمة الملخص. |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


يضبط إعدادات مستوى المقياس الزمني الأوسط للعرض. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | إعدادات مستوى المقياس الزمني الأوسط للعرض. |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


يضبط لون الوقت غير العامل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color | لون الوقت غير العامل. |

### setProgressLines(ProgressLines value) {#setProgressLines-com.aspose.tasks.ProgressLines-}
```
public final void setProgressLines(ProgressLines value)
```


يضبط خطوط التقدم لعرض مخطط Gantt. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ProgressLines](../../com.aspose.tasks/progresslines) | خطوط التقدم لعرض مخطط Gantt. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب تجميع الأشرطة في مخطط جانت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب تجميع الأشرطة على مخطط Gantt. |

### setShowBarSplits(boolean value) {#setShowBarSplits-boolean-}
```
public final void setShowBarSplits(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب إظهار تقسيمات المهام في مخطط جانت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب إظهار تقسيمات المهام على مخطط Gantt. |

### setShowDrawings(boolean value) {#setShowDrawings-boolean-}
```
public final void setShowDrawings(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب إظهار الرسومات في مخطط جانت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب إظهار الرسومات على مخطط Gantt. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


يضبط قائمة من [TextStyle](../../com.aspose.tasks/textstyle) لعرض مخطط جانت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | قائمة من [TextStyle](../../com.aspose.tasks/textstyle) لعرض مخطط Gantt. |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


يضبط نسبة مئوية لتقليل أو تكبير المسافة بين الوحدات في مستوى المقياس الزمني.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | \{@inheritDoc\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


يضبط إعدادات مستوى المقياس الزمني العلوي للعرض. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | إعدادات مستوى المقياس الزمني العلوي للعرض. |

