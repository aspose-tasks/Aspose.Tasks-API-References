---
title: "SaveOptions"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "यह एक अमूर्त बेस क्लास है उन क्लासों के लिए जो उपयोगकर्ता को किसी विशिष्ट फ़ॉर्मेट में परियोजना सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देती हैं।"
type: docs
weight: 274
url: /hi/java/com.aspose.tasks/saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public abstract class SaveOptions extends SimpleSaveOptions
```

यह एक अमूर्त बेस क्लास है उन क्लासों के लिए जो उपयोगकर्ता को किसी विशिष्ट फ़ॉर्मेट में परियोजना सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देती हैं।

--------------------

SaveOptions वर्ग की किसी भी व्युत्पन्न क्लास का एक उदाहरण स्ट्रीम Save या स्ट्रिंग Save ओवरलोड्स को पास किया जाता है ताकि उपयोगकर्ता दस्तावेज़ सहेजते समय कस्टम विकल्प निर्धारित कर सके।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getBarStyles()](#getBarStyles--) | प्रोजेक्ट व्यू में दिखाई देने वाले [BarStyle](../../com.aspose/tasks/barstyle) वर्ग के उदाहरणों की सूची प्राप्त करता है। |
| [getCustomPageSize()](#getCustomPageSize--) | पॉइंट्स में कस्टम पेज आकार प्राप्त करता है (1 पॉइंट = इंच का 1/72)। |
| [getDrawNonWorkingTime()](#getDrawNonWorkingTime--) | एक मान प्राप्त करता है जो दर्शाता है कि गैर-कार्य समय को चित्रित किया जाना चाहिए या नहीं (डिफ़ॉल्ट मान TRUE है)। |
| [getEndDate()](#getEndDate--) | रेंडरिंग समाप्त करने की तिथि प्राप्त करता है। |
| [getFitContent()](#getFitContent--) | एक मान प्राप्त करता है जो दर्शाता है कि पंक्ति की ऊँचाई को उसकी सामग्री के अनुसार बढ़ाया जाना चाहिए या नहीं। |
| [getGridlines()](#getGridlines--) | प्रोजेक्ट व्यू में दिखाई देने वाले [Gridline](../../com.aspose/tasks/gridline) की सूची प्राप्त करता है। |
| [getLegendDrawingOptions()](#getLegendDrawingOptions--) | एक मान प्राप्त करता है जो यह निर्धारित करता है कि लेजेंड कैसे रेंडर किया जाए। |
| [getLegendItems()](#getLegendItems--) | PageLegendItem की एक एरे प्राप्त करता है जो निर्धारित करता है कि पेज लेजेंड में कौन से बार रेंडर किए जाने चाहिए। |
| [getMarkCriticalTasks()](#getMarkCriticalTasks--) | एक मान प्राप्त करता है जो दर्शाता है कि महत्वपूर्ण कार्यों को लाल रंग में दिखाया जाना चाहिए या नहीं (डिफ़ॉल्ट मान FALSE है)। |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | गैर-कार्य समय का रंग प्राप्त करता है। |
| [getPageCount()](#getPageCount--) | प्रोजेक्ट के पृष्ठों की संख्या प्राप्त करता है। |
| [getPageSize()](#getPageSize--) | रेंडर किए जाने वाले पेज का आकार प्राप्त करता है (डिफ़ॉल्ट मान PageSize.A4 है)। |
| [getPresentationFormat()](#getPresentationFormat--) | दस्तावेज़ को सहेजने के लिए उपयोग किए जाने वाले `PresentationFormat`([getPresentationFormat()](../../com.aspose/tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose/tasks/saveoptions\#setPresentationFormat-int-)) को प्राप्त करता है। |
| [getRenderToSinglePage()](#getRenderToSinglePage--) | एक मान प्राप्त करता है जो दर्शाता है कि ग्राफ़िकल फ़ॉर्मेट में प्रोजेक्ट सहेजे जाने पर उसे एक ही पृष्ठ में रेंडर किया जाना चाहिए या नहीं। |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | एक मान प्राप्त करता है जो दर्शाता है कि सारांश टास्क बार पर सबटास्क को चिह्नित किया जाना चाहिए या नहीं। |
| [getStartDate()](#getStartDate--) | रेंडरिंग शुरू करने की तिथि प्राप्त करता है। |
| [getTaskLinkDrawingCallback()](#getTaskLinkDrawingCallback--) | एक कॉलबैक प्राप्त करता है जिसका उपयोग टास्क लिंक रेंडरिंग के कुछ पहलुओं को अनुकूलित करने के लिए किया जा सकता है। |
| [getTextStyles()](#getTextStyles--) | प्रोजेक्ट व्यू के रेंडरिंग के दौरान लागू किए गए टेक्स्ट स्टाइल की सूची प्राप्त करता है। |
| [getTimescale()](#getTimescale--) | `Timescale`([getTimescale()](../../com.aspose/tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose/tasks/saveoptions\#setTimescale-int-)) मान प्राप्त करता है जिसका उपयोग ग्राफ़िकल फ़ॉर्मेट में प्रोजेक्ट सहेजे जाने पर टाइमस्केल (यदि मौजूद हो) को कैसे रेंडर किया जाए, नियंत्रित करने के लिए किया जाता है। |
| [getTimescaleFitBehavior()](#getTimescaleFitBehavior--) | एक व्यवहार प्राप्त करता है जो निर्धारित करता है कि टाइमस्केल के दाएँ सिरे को पृष्ठ के अंत के साथ कैसे संरेखित किया जाए। |
| [getUseGradientBrush()](#getUseGradientBrush--) | एक मान प्राप्त करता है जो दर्शाता है कि गैंट चार्ट रेंडरिंग के समय ग्रेडिएंट ब्रश का उपयोग किया जाना चाहिए या नहीं। |
| [getView()](#getView--) | रेंडर करने के लिए व्यू कॉलम की सूची प्राप्त करता है ([GanttChartColumn](../../com.aspose/tasks/ganttchartcolumn)). |
| [getViewSettings()](#getViewSettings--) | रेंडर करने के लिए एक व्यू (`View`([getView()](../../com.aspose/tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose/tasks/saveoptions\#setView-ProjectView-))) प्राप्त करता है। |
| [isPortrait()](#isPortrait--) | पृष्ठ अभिविन्यास पोर्ट्रेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है; यदि पृष्ठ अभिविन्यास लैंडस्केप है तो false लौटाता है। |
| [setBarStyles(List&lt;BarStyle&gt; value)](#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--) | प्रोजेक्ट व्यू में दिखाई देने वाले [BarStyle](../../com.aspose/tasks/barstyle) क्लास के इंस्टेंस की सूची सेट करता है। |
| [setCustomPageSize(Dimension2D value)](#setCustomPageSize-java.awt.geom.Dimension2D-) | पॉइंट्स में कस्टम पेज आकार सेट करता है (1 पॉइंट = 1/72 इंच)। |
| [setDrawNonWorkingTime(boolean value)](#setDrawNonWorkingTime-boolean-) | एक मान सेट करता है जो दर्शाता है कि गैर-कार्य समय को चित्रित किया जाना चाहिए या नहीं (डिफ़ॉल्ट मान TRUE है)। |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | रेंडरिंग समाप्त करने की तिथि सेट करता है। |
| [setFitContent(boolean value)](#setFitContent-boolean-) | एक मान सेट करता है जो दर्शाता है कि पंक्ति की ऊँचाई को उसकी सामग्री के अनुसार बढ़ाया जाना चाहिए या नहीं। |
| [setGridlines(List&lt;Gridline&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridline--) | प्रोजेक्ट व्यू में दिखाई देने वाले [Gridline](../../com.aspose/tasks/gridline) की सूची सेट करता है। |
| [setLegendDrawingOptions(int value)](#setLegendDrawingOptions-int-) | एक मान सेट करता है जो निर्धारित करता है कि लेजेंड को कैसे रेंडर किया जाए। |
| [setLegendItems(PageLegendItem[] value)](#setLegendItems-com.aspose.tasks.PageLegendItem---) | PageLegendItem की एक एरे सेट करता है जो निर्धारित करता है कि पेज लेजेंड में कौन से बार रेंडर किए जाने चाहिए। |
| [setMarkCriticalTasks(boolean value)](#setMarkCriticalTasks-boolean-) | एक मान सेट करता है जो दर्शाता है कि महत्वपूर्ण टास्क को लाल रंग में दिखाया जाना चाहिए या नहीं (डिफ़ॉल्ट मान FALSE है)। |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | गैर-कार्य समय का रंग सेट करता है। |
| [setPageSize(int value)](#setPageSize-int-) | रेंडर किए जाने वाले पृष्ठ का आकार सेट करता है (डिफ़ॉल्ट मान PageSize.A4 है)। |
| [setPortrait(boolean value)](#setPortrait-boolean-) | पृष्ठ अभिविन्यास पोर्ट्रेट है या नहीं, यह दर्शाने वाला मान सेट करता है; यदि पृष्ठ अभिविन्यास लैंडस्केप है तो false लौटाता है। |
| [setPresentationFormat(int value)](#setPresentationFormat-int-) | `PresentationFormat`([getPresentationFormat()](../../com.aspose/tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose/tasks/saveoptions\#setPresentationFormat-int-)) को सेट करता है जिसमें दस्तावेज़ सहेजा जाएगा। |
| [setRenderToSinglePage(boolean value)](#setRenderToSinglePage-boolean-) | एक मान सेट करता है जो दर्शाता है कि ग्राफ़िकल फ़ॉर्मेट में प्रोजेक्ट सहेजे जाने पर उसे एक ही पृष्ठ में रेंडर किया जाना चाहिए या नहीं। |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | एक मान सेट करता है जो दर्शाता है कि सारांश टास्क बार पर सबटास्क को चिह्नित किया जाना चाहिए या नहीं। |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | रेंडरिंग शुरू करने की तिथि सेट करता है। |
| [setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)](#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-) | टास्क लिंक रेंडरिंग के कुछ पहलुओं को अनुकूलित करने के लिए उपयोग किया जा सकने वाला कॉलबैक सेट करता है। |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | प्रोजेक्ट व्यू के रेंडरिंग के दौरान लागू होने वाले टेक्स्ट स्टाइल की सूची सेट करता है। |
| [setTimescale(int value)](#setTimescale-int-) | प्रोजेक्ट को ग्राफिकल फ़ॉर्मेट में सहेजते समय टाइमस्केल (यदि मौजूद हो) को कैसे रेंडर किया जाता है, इसे नियंत्रित करने के लिए उपयोग किया जाने वाला `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) मान सेट करता है। |
| [setTimescaleFitBehavior(int value)](#setTimescaleFitBehavior-int-) | टाइमस्केल के दाएँ सिरे को पेज के अंत के साथ संरेखित करने का तरीका निर्धारित करने वाला व्यवहार सेट करता है। |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | गैंट चार्ट रेंडरिंग के दौरान ग्रेडिएंट ब्रश का उपयोग किया जाना चाहिए या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | रेंडर करने के लिए व्यू कॉलम की सूची सेट करता है ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [setViewSettings(View value)](#setViewSettings-com.aspose.tasks.View-) | रेंडर करने के लिए एक व्यू (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) सेट करता है। |
### getBarStyles() {#getBarStyles--}
```
public final List<BarStyle> getBarStyles()
```


प्रोजेक्ट व्यू में दिखाई देने वाले [BarStyle](../../com.aspose/tasks/barstyle) वर्ग के उदाहरणों की सूची प्राप्त करता है।

**Returns:**
java.util.List&lt;com.aspose.tasks.BarStyle&gt; - प्रोजेक्ट व्यू में दिखाई देने वाले [BarStyle](../../com.aspose.tasks/barstyle) क्लास के इंस्टेंस की सूची।
### getCustomPageSize() {#getCustomPageSize--}
```
public final Dimension2D getCustomPageSize()
```


पॉइंट्स में कस्टम पेज आकार प्राप्त करता है (1 पॉइंट = इंच का 1/72)।

**Returns:**
java.awt.geom.Dimension2D - पॉइंट्स में कस्टम पेज आकार (1 पॉइंट = इंच का 1/72)।
### getDrawNonWorkingTime() {#getDrawNonWorkingTime--}
```
public final boolean getDrawNonWorkingTime()
```


एक मान प्राप्त करता है जो दर्शाता है कि गैर-कार्य समय को चित्रित किया जाना चाहिए या नहीं (डिफ़ॉल्ट मान TRUE है)।

**Returns:**
boolean - यह दर्शाने वाला मान कि गैर-कार्य समय को ड्रॉ किया जाना चाहिए या नहीं (डिफ़ॉल्ट मान TRUE है)।
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


रेंडरिंग समाप्त करने की तिथि प्राप्त करता है।

**Returns:**
java.util.Date - रेंडरिंग समाप्त करने की तिथि।
### getFitContent() {#getFitContent--}
```
public final boolean getFitContent()
```


एक मान प्राप्त करता है जो दर्शाता है कि पंक्ति की ऊँचाई को उसकी सामग्री के अनुसार बढ़ाया जाना चाहिए या नहीं।

**Returns:**
boolean - यह दर्शाने वाला मान कि पंक्ति की ऊँचाई को उसकी सामग्री फिट करने के लिए बढ़ाया जाना चाहिए या नहीं।
### getGridlines() {#getGridlines--}
```
public final List<Gridline> getGridlines()
```


प्रोजेक्ट व्यू में दिखाई देने वाले [Gridline](../../com.aspose/tasks/gridline) की सूची प्राप्त करता है।

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridline&gt; - प्रोजेक्ट व्यू में दिखाई देने वाले [Gridline](../../com.aspose.tasks/gridline) की सूची।
### getLegendDrawingOptions() {#getLegendDrawingOptions--}
```
public final int getLegendDrawingOptions()
```


एक मान प्राप्त करता है जो यह निर्धारित करता है कि लेजेंड को कैसे रेंडर किया जाए। डिफ़ॉल्ट मान LegendDrawingOptions.OnEveryPage है।

केवल तब लागू होता है जब गैंट चार्ट व्यू रेंडर किया जाता है।

**Returns:**
int - एक मान जो यह निर्धारित करता है कि लेजेंड को कैसे रेंडर किया जाए।
### getLegendItems() {#getLegendItems--}
```
public final PageLegendItem[] getLegendItems()
```


एक एरे प्राप्त करता है जिसमें PageLegendItem होते हैं जो यह निर्धारित करते हैं कि पेज लेजेंड में कौन से बार रेंडर किए जाएँ। यदि null है, तो डिफ़ॉल्ट आइटम रेंडर होते हैं।

केवल तब लागू होता है जब गैंट चार्ट व्यू रेंडर किया जाता है।

**Returns:**
com.aspose.tasks.PageLegendItem[] - एक एरे जिसमें PageLegendItem होते हैं जो यह निर्धारित करते हैं कि पेज लेजेंड में कौन से बार रेंडर किए जाएँ।
### getMarkCriticalTasks() {#getMarkCriticalTasks--}
```
public final boolean getMarkCriticalTasks()
```


एक मान प्राप्त करता है जो दर्शाता है कि महत्वपूर्ण कार्यों को लाल रंग में दिखाया जाना चाहिए या नहीं (डिफ़ॉल्ट मान FALSE है)।

**Returns:**
boolean - यह दर्शाने वाला मान कि महत्वपूर्ण टास्क को लाल रंग में दिखाया जाना चाहिए या नहीं (डिफ़ॉल्ट मान FALSE है)।
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


गैर-कार्य समय का रंग प्राप्त करता है।

**Returns:**
java.awt.Color - गैर-कार्य समय का रंग।
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


प्रोजेक्ट के पृष्ठों की संख्या प्राप्त करता है।

**Returns:**
int - प्रोजेक्ट के पृष्ठों की संख्या।
### getPageSize() {#getPageSize--}
```
public final int getPageSize()
```


रेंडर किए जाने वाले पेज का आकार प्राप्त करता है (डिफ़ॉल्ट मान PageSize.A4 है)।

**Returns:**
int - रेंडर किए जाने वाले पृष्ठ का आकार (डिफ़ॉल्ट मान PageSize.A4 है)।
### getPresentationFormat() {#getPresentationFormat--}
```
public final int getPresentationFormat()
```


दस्तावेज़ को सहेजने के लिए उपयोग किए जाने वाले `PresentationFormat`([getPresentationFormat()](../../com.aspose/tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose/tasks/saveoptions\#setPresentationFormat-int-)) को प्राप्त करता है।

**Returns:**
int - वह `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) जिसमें दस्तावेज़ सहेजा जाएगा।
### getRenderToSinglePage() {#getRenderToSinglePage--}
```
public final boolean getRenderToSinglePage()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि प्रोजेक्ट को ग्राफिकल फ़ॉर्मेट में सहेजते समय एक ही पृष्ठ पर रेंडर किया जाना चाहिए या नहीं। पृष्ठ आकार को इस प्रकार बदल दिया जाएगा कि रेंडर किया गया प्रोजेक्ट एक पृष्ठ में फिट हो सके।

**Returns:**
boolean - एक मान जो दर्शाता है कि प्रोजेक्ट को ग्राफिकल फ़ॉर्मेट में सहेजा जाने पर एक ही पृष्ठ पर रेंडर किया जाना चाहिए या नहीं।
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


एक मान प्राप्त करता है जो दर्शाता है कि सारांश टास्क बार पर सबटास्क को चिह्नित किया जाना चाहिए या नहीं। सबटास्क के लिए, Rollup फ़ील्ड दर्शाता है कि सबटास्क गैंट बार की जानकारी सारांश टास्क बार में रोल अप होगी या नहीं। सारांश टास्क के लिए, Rollup फ़ील्ड दर्शाता है कि सारांश टास्क बार रोल अप बार प्रदर्शित करता है या नहीं। किसी भी सबटास्क को उनके पास रोल अप करने के लिए आपको सारांश टास्क के लिए Rollup फ़ील्ड को Yes पर सेट करना आवश्यक है।

--------------------

केवल तब लागू होता है जब गैंट चार्ट व्यू रेंडर किया जाता है।

**Returns:**
boolean - एक मान जो दर्शाता है कि सारांश टास्क बार पर सबटास्क को चिह्नित किया जाना चाहिए या नहीं।
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


रेंडरिंग शुरू करने की तिथि प्राप्त करता है।

**Returns:**
java.util.Date - वह तिथि जिससे रेंडरिंग शुरू की जानी है।
### getTaskLinkDrawingCallback() {#getTaskLinkDrawingCallback--}
```
public final TaskLinkDrawingCallbackDelegate getTaskLinkDrawingCallback()
```


एक कॉलबैक प्राप्त करता है जिसका उपयोग टास्क लिंक रेंडरिंग के कुछ पहलुओं को अनुकूलित करने के लिए किया जा सकता है।

केवल तब लागू होता है जब गैंट चार्ट व्यू रेंडर किया जाता है।

**Returns:**
[TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) - a callback that can be used to customize some aspects of task links rendering.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


प्रोजेक्ट व्यू के रेंडरिंग के दौरान लागू किए गए टेक्स्ट स्टाइल की सूची प्राप्त करता है।

--------------------

ये शैलियाँ GanttCharView.setTextStyles के साथ परिभाषित शैलियों को ओवरराइड करती हैं।

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - प्रोजेक्ट व्यू के रेंडरिंग के दौरान लागू होने वाली टेक्स्ट शैलियों की सूची।
### getTimescale() {#getTimescale--}
```
public final int getTimescale()
```


`Timescale`([getTimescale()](../../com.aspose/tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose/tasks/saveoptions\#setTimescale-int-)) मान प्राप्त करता है जिसका उपयोग ग्राफ़िकल फ़ॉर्मेट में प्रोजेक्ट सहेजे जाने पर टाइमस्केल (यदि मौजूद हो) को कैसे रेंडर किया जाए, नियंत्रित करने के लिए किया जाता है।

**Returns:**
int - वह `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) मान जो प्रोजेक्ट को ग्राफिकल फ़ॉर्मेट में सहेजते समय टाइमस्केल (यदि मौजूद हो) के रेंडरिंग को नियंत्रित करने के लिए उपयोग किया जाता है।
### getTimescaleFitBehavior() {#getTimescaleFitBehavior--}
```
public final int getTimescaleFitBehavior()
```


एक व्यवहार प्राप्त करता है जो निर्धारित करता है कि टाइमस्केल के दाएँ सिरे को पृष्ठ के अंत के साथ कैसे संरेखित किया जाए।

**Returns:**
int - एक व्यवहार जो निर्धारित करता है कि टाइमस्केल के दाएँ अंत को पृष्ठ के अंत के साथ कैसे संरेखित किया जाए।
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


एक मान प्राप्त करता है जो दर्शाता है कि गैंट चार्ट रेंडरिंग के समय ग्रेडिएंट ब्रश का उपयोग किया जाना चाहिए या नहीं।

--------------------

केवल तब लागू होता है जब गैंट चार्ट व्यू रेंडर किया जाता है।

**Returns:**
boolean - एक मान जो दर्शाता है कि गैंट चार्ट रेंडर करते समय ग्रेडिएंट ब्रश का उपयोग किया जाना चाहिए या नहीं।
### getView() {#getView--}
```
public final ProjectView getView()
```


रेंडर करने के लिए व्यू कॉलम की सूची प्राप्त करता है ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). यदि सेट नहीं किया गया है तो केवल टास्क आईडी, टास्क नाम, शुरू और समाप्ति रेंडर होते हैं। यदि दोनों View और `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) प्रॉपर्टीज़ सेट हैं, तो View से कॉलम ViewSettings के कॉलम को ओवरराइड करते हैं।

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)).
### getViewSettings() {#getViewSettings--}
```
public final View getViewSettings()
```


रेंडर करने के लिए एक व्यू (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) प्राप्त करता है। आप इस विकल्प का उपयोग करके स्पष्ट रूप से निर्दिष्ट कर सकते हैं कि कौन सा व्यू PDF, HTML या इमेज फ़ॉर्मेट में सहेजा जाना चाहिए। यदि यह प्रॉपर्टी सेट है, तो प्रोजेक्ट सहेजते समय [PresentationFormat](../../com.aspose.tasks/presentationformat) प्रॉपर्टी को अनदेखा किया जाता है। व्यू निम्नलिखित स्क्रीन में से किसी एक का होना चाहिए ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Returns:**
[View](../../com.aspose.tasks/view) - a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


पृष्ठ अभिविन्यास पोर्ट्रेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है; यदि पृष्ठ अभिविन्यास लैंडस्केप है तो false लौटाता है।

--------------------

जब SaveOptions.getPageSize() == PageSize.DefinedInView हो तो लागू नहीं होता। इस मामले में [PageSettings.isPortrait()](../../com.aspose.tasks/pagesettings\#isPortrait--) का उपयोग किया जाता है। जब [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) सेट हो तो भी लागू नहीं होता।

**Returns:**
boolean - यह दर्शाने वाला मान कि पेज अभिविन्यास पोर्ट्रेट है; यदि पेज अभिविन्यास लैंडस्केप है तो false लौटाता है।
### setBarStyles(List&lt;BarStyle&gt; value) {#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--}
```
public final void setBarStyles(List<BarStyle> value)
```


प्रोजेक्ट व्यू में दिखाई देने वाले [BarStyle](../../com.aspose/tasks/barstyle) क्लास के इंस्टेंस की सूची सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.BarStyle&gt; | प्रोजेक्ट व्यू में दिखाई देने वाले [BarStyle](../../com.aspose.tasks/barstyle) क्लास के इंस्टेंस की सूची। |

### setCustomPageSize(Dimension2D value) {#setCustomPageSize-java.awt.geom.Dimension2D-}
```
public final void setCustomPageSize(Dimension2D value)
```


पॉइंट्स में कस्टम पेज आकार सेट करता है (1 पॉइंट = 1/72 इंच)।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.awt.geom.Dimension2D | पॉइंट्स में कस्टम पेज आकार (1 पॉइंट = 1/72 इंच)। |

### setDrawNonWorkingTime(boolean value) {#setDrawNonWorkingTime-boolean-}
```
public final void setDrawNonWorkingTime(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि गैर-कार्य समय को चित्रित किया जाना चाहिए या नहीं (डिफ़ॉल्ट मान TRUE है)।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि गैर-कार्य समय को ड्रॉ किया जाना चाहिए या नहीं (डिफ़ॉल्ट मान TRUE है)। |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


रेंडरिंग समाप्त करने की तिथि सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | रेंडरिंग समाप्त करने की तिथि। |

### setFitContent(boolean value) {#setFitContent-boolean-}
```
public final void setFitContent(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि पंक्ति की ऊँचाई को उसकी सामग्री के अनुसार बढ़ाया जाना चाहिए या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि पंक्ति की ऊँचाई को उसकी सामग्री में फिट करने के लिए बढ़ाया जाना चाहिए या नहीं। |

### setGridlines(List&lt;Gridline&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridline--}
```
public final void setGridlines(List<Gridline> value)
```


प्रोजेक्ट व्यू में दिखाई देने वाले [Gridline](../../com.aspose/tasks/gridline) की सूची सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridline&gt; | प्रोजेक्ट व्यू में दिखाई देने वाले [Gridline](../../com.aspose.tasks/gridline) की सूची। |

### setLegendDrawingOptions(int value) {#setLegendDrawingOptions-int-}
```
public final void setLegendDrawingOptions(int value)
```


एक मान सेट करता है जो परिभाषित करता है कि लेजेंड को कैसे रेंडर किया जाए। डिफ़ॉल्ट मान LegendDrawingOptions.OnEveryPage है।

केवल तब लागू होता है जब गैंट चार्ट व्यू रेंडर किया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | एक मान जो परिभाषित करता है कि लेजेंड को कैसे रेंडर किया जाए। |

### setLegendItems(PageLegendItem[] value) {#setLegendItems-com.aspose.tasks.PageLegendItem---}
```
public final void setLegendItems(PageLegendItem[] value)
```


एक एरे सेट करता है जिसमें PageLegendItem होते हैं जो परिभाषित करते हैं कि पेज लेजेंड में कौन से बार रेंडर किए जाने चाहिए। यदि null है, तो डिफ़ॉल्ट आइटम रेंडर होते हैं।

केवल तब लागू होता है जब गैंट चार्ट व्यू रेंडर किया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [PageLegendItem\[\]](../../com.aspose.tasks/pagelegenditem) | PageLegendItem का एक एरे जो परिभाषित करता है कि पेज लेजेंड में कौन से बार रेंडर किए जाने चाहिए। |

### setMarkCriticalTasks(boolean value) {#setMarkCriticalTasks-boolean-}
```
public final void setMarkCriticalTasks(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि महत्वपूर्ण टास्क को लाल रंग में दिखाया जाना चाहिए या नहीं (डिफ़ॉल्ट मान FALSE है)।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि महत्वपूर्ण टास्क को लाल रंग में दिखाया जाना चाहिए या नहीं (डिफ़ॉल्ट मान FALSE है)। |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


गैर-कार्य समय का रंग सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.awt.Color | गैर-कार्य समय का रंग। |

### setPageSize(int value) {#setPageSize-int-}
```
public final void setPageSize(int value)
```


रेंडर किए जाने वाले पृष्ठ का आकार सेट करता है (डिफ़ॉल्ट मान PageSize.A4 है)।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | रेंडर किए जाने वाले पृष्ठ का आकार (डिफ़ॉल्ट मान PageSize.A4 है)। |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


पृष्ठ अभिविन्यास पोर्ट्रेट है या नहीं, यह दर्शाने वाला मान सेट करता है; यदि पृष्ठ अभिविन्यास लैंडस्केप है तो false लौटाता है।

--------------------

जब SaveOptions.PageSize == Visualization.PageSize.DefinedInView हो, तब लागू नहीं होता। इस स्थिति में [PageSettings.setPortrait(boolean)](../../com.aspose.tasks/pagesettings\#setPortrait-boolean-) का उपयोग किया जाता है। जब [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) सेट किया जाता है, तब भी लागू नहीं होता।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | पेज अभिविन्यास पोर्ट्रेट है या नहीं, यह दर्शाने वाला मान; यदि पेज अभिविन्यास लैंडस्केप है तो false लौटाता है। |

### setPresentationFormat(int value) {#setPresentationFormat-int-}
```
public final void setPresentationFormat(int value)
```


`PresentationFormat`([getPresentationFormat()](../../com.aspose/tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose/tasks/saveoptions\#setPresentationFormat-int-)) को सेट करता है जिसमें दस्तावेज़ सहेजा जाएगा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | int | वह `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) जिसमें दस्तावेज़ सहेजा जाएगा। |

### setRenderToSinglePage(boolean value) {#setRenderToSinglePage-boolean-}
```
public final void setRenderToSinglePage(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि जब प्रोजेक्ट को ग्राफिकल फ़ॉर्मेट में सहेजा जाता है तो उसे एक पृष्ठ पर रेंडर किया जाना चाहिए या नहीं। पृष्ठ आकार बदल दिया जाएगा ताकि रेंडर किया गया प्रोजेक्ट एक पृष्ठ में फिट हो सके।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि जब प्रोजेक्ट को ग्राफिकल फ़ॉर्मेट में सहेजा जाता है तो उसे एक पृष्ठ पर रेंडर किया जाना चाहिए या नहीं। |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि सारांश टास्क बार पर सबटास्क को चिह्नित किया जाना चाहिए या नहीं। सबटास्क के लिए, Rollup फ़ील्ड यह दर्शाता है कि सबटास्क गैंट बार की जानकारी सारांश टास्क बार में रोल अप होगी या नहीं। सारांश टास्क के लिए, Rollup फ़ील्ड यह दर्शाता है कि सारांश टास्क बार रोल अप बार प्रदर्शित करता है या नहीं। किसी भी सबटास्क को उनके पास रोल अप करने के लिए आपको सारांश टास्क के लिए Rollup फ़ील्ड को Yes पर सेट करना होगा।

--------------------

केवल तब लागू होता है जब गैंट चार्ट व्यू रेंडर किया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि सारांश टास्क बार पर सबटास्क को चिह्नित किया जाना चाहिए या नहीं। |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


रेंडरिंग शुरू करने की तिथि सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | रेंडरिंग शुरू करने की तिथि। |

### setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value) {#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-}
```
public final void setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)
```


टास्क लिंक रेंडरिंग के कुछ पहलुओं को अनुकूलित करने के लिए उपयोग किया जा सकने वाला कॉलबैक सेट करता है।

केवल तब लागू होता है जब गैंट चार्ट व्यू रेंडर किया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) | एक कॉलबैक जो टास्क लिंक रेंडरिंग के कुछ पहलुओं को अनुकूलित करने के लिए उपयोग किया जा सकता है। |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


प्रोजेक्ट व्यू के रेंडरिंग के दौरान लागू होने वाले टेक्स्ट स्टाइल की सूची सेट करता है।

--------------------

ये शैलियाँ GanttCharView.setTextStyles के साथ परिभाषित शैलियों को ओवरराइड करती हैं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | प्रोजेक्ट व्यू के रेंडरिंग के दौरान लागू होने वाले टेक्स्ट स्टाइल की सूची। |

### setTimescale(int value) {#setTimescale-int-}
```
public final void setTimescale(int value)
```


प्रोजेक्ट को ग्राफिकल फ़ॉर्मेट में सहेजते समय टाइमस्केल (यदि मौजूद हो) को कैसे रेंडर किया जाता है, इसे नियंत्रित करने के लिए उपयोग किया जाने वाला `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | int | वह `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) मान जिसका उपयोग यह नियंत्रित करने के लिए किया जाता है कि प्रोजेक्ट को ग्राफिकल फ़ॉर्मेट में सहेजते समय टाइमस्केल (यदि मौजूद हो) कैसे रेंडर किया जाता है। |

### setTimescaleFitBehavior(int value) {#setTimescaleFitBehavior-int-}
```
public final void setTimescaleFitBehavior(int value)
```


टाइमस्केल के दाएँ सिरे को पेज के अंत के साथ संरेखित करने का तरीका निर्धारित करने वाला व्यवहार सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | एक व्यवहार जो निर्धारित करता है कि टाइमस्केल के दाएँ सिरे को पृष्ठ के अंत के साथ कैसे संरेखित किया जाए। |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


गैंट चार्ट रेंडरिंग के दौरान ग्रेडिएंट ब्रश का उपयोग किया जाना चाहिए या नहीं, यह दर्शाने वाला मान सेट करता है।

--------------------

केवल तब लागू होता है जब गैंट चार्ट व्यू रेंडर किया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि गैंट चार्ट रेंडरिंग के समय ग्रेडिएंट ब्रश का उपयोग किया जाना चाहिए या नहीं। |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


रेंडर करने के लिए व्यू कॉलम की सूची सेट करता है ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). यदि सेट नहीं किया गया तो केवल टास्क आईडी, टास्क नाम, प्रारंभ और समाप्ति रेंडर होते हैं। यदि View और `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) दोनों प्रॉपर्टी सेट हैं, तो View से कॉलम ViewSettings के कॉलमों को ओवरराइड कर देते हैं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | रेंडर करने के लिए व्यू कॉलम की सूची ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |

### setViewSettings(View value) {#setViewSettings-com.aspose.tasks.View-}
```
public final void setViewSettings(View value)
```


रेंडर करने के लिए एक व्यू (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) सेट करता है। आप इस विकल्प का उपयोग करके स्पष्ट रूप से निर्दिष्ट कर सकते हैं कि कौन सा व्यू PDF, HTML या Image फ़ॉर्मेट में सहेजा जाना चाहिए। यदि यह प्रॉपर्टी सेट है, तो प्रोजेक्ट सहेजे जाने पर [PresentationFormat](../../com.aspose.tasks/presentationformat) प्रॉपर्टी को अनदेखा किया जाता है। व्यू निम्नलिखित स्क्रीन में से किसी एक का होना चाहिए ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | रेंडर करने के लिए एक व्यू (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-)))। |

