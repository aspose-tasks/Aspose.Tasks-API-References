---
title: "GanttChartView"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "गैंटचार्ट दृश्य का प्रतिनिधित्व करता है।"
type: docs
weight: 112
url: /hi/java/com.aspose.tasks/ganttchartview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public class GanttChartView extends View implements ITimescaledView
```

गैंटचार्ट दृश्य का प्रतिनिधित्व करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [GanttChartView()](#GanttChartView--) | एक नया उदाहरण प्रारंभ करता है [GanttChartView](../../com.aspose.tasks/ganttchartview) क्लास का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getAutoFilters()](#getAutoFilters--) | Gantt Chart दृश्य के ऑटो फ़िल्टरों की सूची प्राप्त करता है। |
| [getBarRounding()](#getBarRounding--) | बारों को निकटतम दिन तक गोल करने का संकेत देने वाला मान प्राप्त करता है। |
| [getBarSize()](#getBarSize--) | Gantt Chart में Gantt बारों की ऊँचाई, पॉइंट्स में, प्राप्त करता है। |
| [getBarStyles()](#getBarStyles--) | Gantt Chart दृश्य के पैरेंट (सामान्य) बार शैलियों की सूची प्राप्त करता है। |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | व्यू के नीचे के टाइमस्केल टियर की सेटिंग्स प्राप्त करता है। |
| [getCustomBarStyles()](#getCustomBarStyles--) | Gantt Chart दृश्य के कस्टम टास्क-विशिष्ट बार शैलियों की सूची प्राप्त करता है। |
| [getGridlines()](#getGridlines--) | Gantt Chart दृश्य के `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) की सूची प्राप्त करता है। |
| [getHideRollupBarsWhenSummaryExpanded()](#getHideRollupBarsWhenSummaryExpanded--) | रोलअप बारों को सारांश टास्क का विस्तार करते समय छिपाया जाएगा या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | व्यू के मध्य टाइमस्केल टियर की सेटिंग्स प्राप्त करता है। |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | गैर-कार्य समय का रंग प्राप्त करता है। |
| [getProgressLines()](#getProgressLines--) | Gantt Chart दृश्य के लिए प्रोग्रेस लाइनों को प्राप्त करता है। |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Gantt Chart पर बारों को रोल अप करना आवश्यक है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getShowBarSplits()](#getShowBarSplits--) | Gantt Chart पर टास्क विभाजन दिखाए जाने चाहिए या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getShowDrawings()](#getShowDrawings--) | Gantt Chart पर ड्रॉइंग्स दिखाए जाने चाहिए या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getTableTextStyles()](#getTableTextStyles--) | Gantt Chart दृश्य के टेबल टेक्स्ट शैलियों की सूची प्राप्त करता है। |
| [getTextStyles()](#getTextStyles--) | Gantt Chart दृश्य के [TextStyle](../../com.aspose.tasks/textstyle) की सूची प्राप्त करता है। |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \{@inheritDoc\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | व्यू के शीर्ष टाइमस्केल टियर की सेटिंग्स प्राप्त करता है। |
| [setBarRounding(boolean value)](#setBarRounding-boolean-) | बारों को निकटतम दिन तक गोल करने का संकेत देने वाला मान सेट करता है। |
| [setBarSize(int value)](#setBarSize-int-) | Gantt Chart में Gantt बारों की ऊँचाई, पॉइंट्स में, सेट करता है। |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | व्यू के नीचे के टाइमस्केल टियर की सेटिंग्स सेट करता है। |
| [setGridlines(List&lt;Gridlines&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridlines--) | Gantt Chart दृश्य के लिए `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) की सूची सेट करता है। |
| [setHideRollupBarsWhenSummaryExpanded(boolean value)](#setHideRollupBarsWhenSummaryExpanded-boolean-) | सारांश कार्य का विस्तार करते समय रोलअप बार छिपाए जाएंगे या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | दृश्य की मध्य टाइमस्केल टियर की सेटिंग्स सेट करता है। |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | गैर-कार्य समय का रंग सेट करता है। |
| [setProgressLines(ProgressLines value)](#setProgressLines-com.aspose.tasks.ProgressLines-) | Gantt Chart दृश्य के लिए प्रोग्रेस लाइन्स सेट करता है। |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Gantt Chart पर बार को रोल अप करना आवश्यक है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setShowBarSplits(boolean value)](#setShowBarSplits-boolean-) | Gantt Chart पर टास्क स्प्लिट्स दिखाए जाने चाहिए या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setShowDrawings(boolean value)](#setShowDrawings-boolean-) | Gantt Chart पर ड्रॉइंग्स दिखाए जाने चाहिए या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Gantt Chart दृश्य के लिए [TextStyle](../../com.aspose.tasks/textstyle) की सूची सेट करता है। |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \{@inheritDoc\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | दृश्य की शीर्ष टाइमस्केल टियर की सेटिंग्स सेट करता है। |
### GanttChartView() {#GanttChartView--}
```
public GanttChartView()
```


एक नया उदाहरण प्रारंभ करता है [GanttChartView](../../com.aspose.tasks/ganttchartview) क्लास का।

### getAutoFilters() {#getAutoFilters--}
```
public final FilterCollection getAutoFilters()
```


Gantt Chart दृश्य के ऑटो फ़िल्टरों की सूची प्राप्त करता है।

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - a list of auto filters of a Gantt Chart view.
### getBarRounding() {#getBarRounding--}
```
public final boolean getBarRounding()
```


बार को निकटतम दिन तक गोल करने का संकेत देने वाला मान प्राप्त करता है। डिफ़ॉल्ट मान True है।

**Returns:**
boolean - बार को निकटतम दिन तक गोल करने का संकेत देने वाला मान।
### getBarSize() {#getBarSize--}
```
public final int getBarSize()
```


Gantt Chart में Gantt बारों की ऊँचाई, पॉइंट्स में, प्राप्त करता है।

**Returns:**
int - Gantt Chart में Gantt बार की ऊँचाई, पॉइंट्स में।
### getBarStyles() {#getBarStyles--}
```
public final List<GanttBarStyle> getBarStyles()
```


Gantt Chart दृश्य के पैरेंट (सामान्य) बार शैलियों की सूची प्राप्त करता है। [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - Gantt Chart दृश्य के पैरेंट (सामान्य) बार शैलियों की सूची।
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


दृश्य की निचली टाइमस्केल टियर की सेटिंग्स प्राप्त करता है। [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getCustomBarStyles() {#getCustomBarStyles--}
```
public final List<GanttBarStyle> getCustomBarStyles()
```


Gantt Chart दृश्य के कस्टम टास्क-विशिष्ट बार शैलियों की सूची प्राप्त करता है। [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - Gantt Chart दृश्य के कस्टम टास्क-विशिष्ट बार शैलियों की सूची।
### getGridlines() {#getGridlines--}
```
public final List<Gridlines> getGridlines()
```


Gantt Chart दृश्य के `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) की सूची प्राप्त करता है।

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridlines&gt; - Gantt Chart दृश्य के `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) की सूची।
### getHideRollupBarsWhenSummaryExpanded() {#getHideRollupBarsWhenSummaryExpanded--}
```
public final boolean getHideRollupBarsWhenSummaryExpanded()
```


रोलअप बारों को सारांश टास्क का विस्तार करते समय छिपाया जाएगा या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - सारांश कार्य का विस्तार करते समय रोलअप बार छिपाए जाएंगे या नहीं, यह दर्शाने वाला मान।
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


दृश्य की मध्य टाइमस्केल टियर की सेटिंग्स प्राप्त करता है। [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


गैर-कार्य समय का रंग प्राप्त करता है।

**Returns:**
java.awt.Color - गैर-कार्य समय का रंग।
### getProgressLines() {#getProgressLines--}
```
public final ProgressLines getProgressLines()
```


Gantt Chart दृश्य के लिए प्रोग्रेस लाइन्स प्राप्त करता है। `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Returns:**
[ProgressLines](../../com.aspose.tasks/progresslines) - progress lines for the Gantt Chart view.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Gantt Chart पर बारों को रोल अप करना आवश्यक है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - Gantt Chart पर बार को रोल अप करना आवश्यक है या नहीं, यह दर्शाने वाला मान।
### getShowBarSplits() {#getShowBarSplits--}
```
public final boolean getShowBarSplits()
```


Gantt Chart पर टास्क विभाजन दिखाए जाने चाहिए या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - Gantt Chart पर टास्क स्प्लिट्स दिखाए जाने चाहिए या नहीं, यह दर्शाने वाला मान।
### getShowDrawings() {#getShowDrawings--}
```
public final boolean getShowDrawings()
```


Gantt Chart पर ड्रॉइंग्स दिखाए जाने चाहिए या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - Gantt Chart पर ड्रॉइंग्स दिखाए जाने चाहिए या नहीं, यह दर्शाने वाला मान।
### getTableTextStyles() {#getTableTextStyles--}
```
public final List<TableTextStyle> getTableTextStyles()
```


Gantt Chart दृश्य के टेबल टेक्स्ट शैलियों की सूची प्राप्त करता है। [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.TableTextStyle&gt; - Gantt Chart दृश्य के टेबल टेक्स्ट शैलियों की सूची।
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Gantt Chart दृश्य के [TextStyle](../../com.aspose.tasks/textstyle) की सूची प्राप्त करता है।

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - Gantt Chart दृश्य के [TextStyle](../../com.aspose.tasks/textstyle) की सूची।
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


टाइमस्केल टियर पर इकाइयों के बीच की दूरी को घटाने या बढ़ाने के लिए प्रतिशत प्राप्त करता है।

**Returns:**
int - \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


दृश्य की शीर्ष टाइमस्केल टियर की सेटिंग्स प्राप्त करता है। [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setBarRounding(boolean value) {#setBarRounding-boolean-}
```
public final void setBarRounding(boolean value)
```


बारों को निकटतम दिन तक गोल करने का संकेत देने वाला मान सेट करता है। डिफ़ॉल्ट मान True है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | बारों को निकटतम दिन तक गोल करने का संकेत देने वाला मान। |

### setBarSize(int value) {#setBarSize-int-}
```
public final void setBarSize(int value)
```


Gantt Chart में Gantt बारों की ऊँचाई, पॉइंट्स में, सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | Gantt चार्ट में Gantt बारों की ऊँचाई, पॉइंट्स में। |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


दृश्य की निचली टाइमस्केल टियर की सेटिंग्स सेट करता है। [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | दृश्य की निचली टाइमस्केल टियर की सेटिंग्स। |

### setGridlines(List&lt;Gridlines&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridlines--}
```
public final void setGridlines(List<Gridlines> value)
```


Gantt Chart दृश्य के लिए `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) की सूची सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridlines&gt; | Gantt चार्ट दृश्य की `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) की सूची। |

### setHideRollupBarsWhenSummaryExpanded(boolean value) {#setHideRollupBarsWhenSummaryExpanded-boolean-}
```
public final void setHideRollupBarsWhenSummaryExpanded(boolean value)
```


सारांश कार्य का विस्तार करते समय रोलअप बार छिपाए जाएंगे या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | सारांश कार्य को विस्तारित करने पर रोलअप बारों को छिपाया जाएगा या नहीं, यह दर्शाने वाला मान। |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


दृश्य की मध्य टाइमस्केल टियर की सेटिंग्स सेट करता है। [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | दृश्य की मध्य टाइमस्केल टियर की सेटिंग्स। |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


गैर-कार्य समय का रंग सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.awt.Color | गैर-कार्य समय का रंग। |

### setProgressLines(ProgressLines value) {#setProgressLines-com.aspose.tasks.ProgressLines-}
```
public final void setProgressLines(ProgressLines value)
```


Gantt चार्ट दृश्य के लिए प्रोग्रेस लाइन्स सेट करता है। `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [ProgressLines](../../com.aspose.tasks/progresslines) | Gantt चार्ट दृश्य के लिए प्रोग्रेस लाइन्स। |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Gantt Chart पर बार को रोल अप करना आवश्यक है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | Gantt चार्ट पर बारों को रोल अप करना आवश्यक है या नहीं, यह दर्शाने वाला मान। |

### setShowBarSplits(boolean value) {#setShowBarSplits-boolean-}
```
public final void setShowBarSplits(boolean value)
```


Gantt Chart पर टास्क स्प्लिट्स दिखाए जाने चाहिए या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | Gantt चार्ट पर टास्क स्प्लिट्स दिखाए जाने चाहिए या नहीं, यह दर्शाने वाला मान। |

### setShowDrawings(boolean value) {#setShowDrawings-boolean-}
```
public final void setShowDrawings(boolean value)
```


Gantt Chart पर ड्रॉइंग्स दिखाए जाने चाहिए या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | Gantt चार्ट पर ड्रॉइंग्स दिखाए जाने चाहिए या नहीं, यह दर्शाने वाला मान। |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Gantt Chart दृश्य के लिए [TextStyle](../../com.aspose.tasks/textstyle) की सूची सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | Gantt चार्ट दृश्य की [TextStyle](../../com.aspose.tasks/textstyle) की सूची। |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


टाइमस्केल टियर पर इकाइयों के बीच की दूरी को घटाने या बढ़ाने के लिए प्रतिशत सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | \{@inheritDoc\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


दृश्य की शीर्ष टाइमस्केल टियर की सेटिंग्स सेट करता है। [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | दृश्य की शीर्ष टाइमस्केल टियर की सेटिंग्स। |

