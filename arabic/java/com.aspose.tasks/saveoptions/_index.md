---
title: "SaveOptions"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "هذه فئة أساسية مجردة للفئات التي تسمح للمستخدم بتحديد خيارات إضافية عند حفظ مشروع بتنسيق معين."
type: docs
weight: 274
url: /ar/java/com.aspose.tasks/saveoptions/
---

**Inheritance:**
java.lang.Object، [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public abstract class SaveOptions extends SimpleSaveOptions
```

هذه فئة أساسية مجردة للفئات التي تسمح للمستخدم بتحديد خيارات إضافية عند حفظ مشروع بتنسيق معين.

--------------------

يتم تمرير نسخة من أي فئة مشتقة من الفئة SaveOptions إلى عمليات التحميل عبر الدفق Save أو السلسلة Save لتحديد خيارات مخصصة عند حفظ المستند.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getBarStyles()](#getBarStyles--) | يحصل على قائمة بنُسخ الفئة [BarStyle](../../com.aspose.tasks/barstyle) التي تظهر في عرض المشروع. |
| [getCustomPageSize()](#getCustomPageSize--) | يحصل على حجم الصفحة المخصص بالنقاط (1 نقطة = 1/72 بوصة). |
| [getDrawNonWorkingTime()](#getDrawNonWorkingTime--) | يحصل على قيمة تشير إلى ما إذا كان يجب رسم الوقت غير العامل (القيمة الافتراضية هي TRUE). |
| [getEndDate()](#getEndDate--) | يحصل على تاريخ لإنهاء العرض إليه. |
| [getFitContent()](#getFitContent--) | يحصل على قيمة تشير إلى ما إذا كان يجب زيادة ارتفاع الصف ليتناسب مع محتواه. |
| [getGridlines()](#getGridlines--) | يحصل على قائمة بـ [Gridline](../../com.aspose.tasks/gridline) التي تظهر في عرض المشروع. |
| [getLegendDrawingOptions()](#getLegendDrawingOptions--) | يحصل على قيمة تحدد طريقة عرض المفتاح. |
| [getLegendItems()](#getLegendItems--) | يحصل على مصفوفة من PageLegendItem التي تحدد أي الأشرطة يجب عرضها في مفتاح الصفحة. |
| [getMarkCriticalTasks()](#getMarkCriticalTasks--) | يحصل على قيمة تشير إلى ما إذا كان يجب عرض المهام الحرجة باللون الأحمر (القيمة الافتراضية هي FALSE). |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | يحصل على لون الوقت غير العامل. |
| [getPageCount()](#getPageCount--) | يحصل على عدد صفحات المشروع. |
| [getPageSize()](#getPageSize--) | يحصل على حجم الصفحة التي سيتم عرضها (القيمة الافتراضية هي PageSize.A4). |
| [getPresentationFormat()](#getPresentationFormat--) | يحصل على `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) التي سيتم حفظ المستند بها. |
| [getRenderToSinglePage()](#getRenderToSinglePage--) | يحصل على قيمة تشير إلى ما إذا كان يجب عرض المشروع في صفحة واحدة عندما يتم حفظ المشروع بتنسيق رسومي. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | يحصل على قيمة تشير إلى ما إذا كان يجب وضع علامة على المهام الفرعية في شريط المهمة الملخصة. |
| [getStartDate()](#getStartDate--) | يحصل على التاريخ الذي يبدأ منه العرض. |
| [getTaskLinkDrawingCallback()](#getTaskLinkDrawingCallback--) | يحصل على رد نداء يمكن استخدامه لتخصيص بعض جوانب عرض روابط المهام. |
| [getTextStyles()](#getTextStyles--) | يحصل على قائمة أنماط النص التي تُطبق أثناء عرض منظور المشروع. |
| [getTimescale()](#getTimescale--) | يحصل على قيمة `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) التي تُستخدم للتحكم في كيفية عرض المقياس الزمني (إن وجد) عندما يتم حفظ المشروع بتنسيق رسومي. |
| [getTimescaleFitBehavior()](#getTimescaleFitBehavior--) | يحصل على سلوك يحدد كيفية محاذاة الطرف الأيمن للمقياس الزمني مع نهاية الصفحة. |
| [getUseGradientBrush()](#getUseGradientBrush--) | يحصل على قيمة تشير إلى ما إذا كان يجب استخدام فرشاة التدرج عند عرض مخطط جانت. |
| [getView()](#getView--) | يحصل على قائمة أعمدة العرض التي سيتم عرضها ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [getViewSettings()](#getViewSettings--) | يحصل على منظور (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) للعرض. |
| [isPortrait()](#isPortrait--) | يحصل على قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا؛ يعيد false إذا كان اتجاه الصفحة أفقيًا. |
| [setBarStyles(List&lt;BarStyle&gt; value)](#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--) | يضبط قائمة مثيلات الفئة [BarStyle](../../com.aspose.tasks/barstyle) التي تظهر في منظور المشروع. |
| [setCustomPageSize(Dimension2D value)](#setCustomPageSize-java.awt.geom.Dimension2D-) | يضبط حجم الصفحة المخصص بالنقاط (نقطة واحدة = 1/72 بوصة). |
| [setDrawNonWorkingTime(boolean value)](#setDrawNonWorkingTime-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب رسم وقت غير العمل (القيمة الافتراضية هي TRUE). |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | يضبط تاريخ الانتهاء من العرض. |
| [setFitContent(boolean value)](#setFitContent-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب زيادة ارتفاع الصف ليتناسب مع محتواه. |
| [setGridlines(List&lt;Gridline&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridline--) | يضبط قائمة [Gridline](../../com.aspose.tasks/gridline) التي تظهر في منظور المشروع. |
| [setLegendDrawingOptions(int value)](#setLegendDrawingOptions-int-) | يضبط قيمة تحدد كيفية عرض مفتاح الشرح. |
| [setLegendItems(PageLegendItem[] value)](#setLegendItems-com.aspose.tasks.PageLegendItem---) | يضبط مصفوفة PageLegendItem التي تحدد أي الأشرطة يجب عرضها في مفتاح الشرح للصفحة. |
| [setMarkCriticalTasks(boolean value)](#setMarkCriticalTasks-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب عرض المهام الحرجة باللون الأحمر (القيمة الافتراضية هي FALSE). |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | يضبط لون وقت غير العمل. |
| [setPageSize(int value)](#setPageSize-int-) | يضبط حجم الصفحة التي سيتم عرضها (القيمة الافتراضية هي PageSize.A4). |
| [setPortrait(boolean value)](#setPortrait-boolean-) | يضبط قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا؛ يعيد false إذا كان اتجاه الصفحة أفقيًا. |
| [setPresentationFormat(int value)](#setPresentationFormat-int-) | يضبط `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) التي سيتم حفظ المستند بها. |
| [setRenderToSinglePage(boolean value)](#setRenderToSinglePage-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب عرض المشروع في صفحة واحدة عندما يتم حفظ المشروع بتنسيق رسومي. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب وضع علامة على المهام الفرعية في شريط المهمة الملخصة. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | يضبط التاريخ للبدء في العرض من. |
| [setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)](#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-) | يضبط رد نداء يمكن استخدامه لتخصيص بعض جوانب عرض روابط المهام. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | يضبط قائمة أنماط النص التي تُطبق أثناء عرض منظور المشروع. |
| [setTimescale(int value)](#setTimescale-int-) | يضبط قيمة `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) التي تُستخدم للتحكم في كيفية عرض المقياس الزمني (إن وجد) عند حفظ المشروع بتنسيق رسومي. |
| [setTimescaleFitBehavior(int value)](#setTimescaleFitBehavior-int-) | يضبط سلوكًا يحدد كيفية محاذاة الطرف الأيمن للمقياس الزمني مع نهاية الصفحة. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب استخدام فرشاة التدرج عند عرض مخطط جانت. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | يضبط قائمة أعمدة العرض التي سيتم عرضها ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [setViewSettings(View value)](#setViewSettings-com.aspose.tasks.View-) | يضبط منظورًا (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) للعرض. |
### getBarStyles() {#getBarStyles--}
```
public final List<BarStyle> getBarStyles()
```


يحصل على قائمة بنُسخ الفئة [BarStyle](../../com.aspose.tasks/barstyle) التي تظهر في عرض المشروع.

**Returns:**
java.util.List&lt;com.aspose.tasks.BarStyle&gt; - قائمة كائنات فئة [BarStyle](../../com.aspose.tasks/barstyle) التي تظهر في منظور المشروع.
### getCustomPageSize() {#getCustomPageSize--}
```
public final Dimension2D getCustomPageSize()
```


يحصل على حجم الصفحة المخصص بالنقاط (1 نقطة = 1/72 بوصة).

**Returns:**
java.awt.geom.Dimension2D - حجم الصفحة المخصص بالنقاط (1 نقطة = 1/72 بوصة).
### getDrawNonWorkingTime() {#getDrawNonWorkingTime--}
```
public final boolean getDrawNonWorkingTime()
```


يحصل على قيمة تشير إلى ما إذا كان يجب رسم الوقت غير العامل (القيمة الافتراضية هي TRUE).

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب رسم الوقت غير العامل (القيمة الافتراضية هي TRUE).
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


يحصل على تاريخ لإنهاء العرض إليه.

**Returns:**
java.util.Date - تاريخ الانتهاء من العرض.
### getFitContent() {#getFitContent--}
```
public final boolean getFitContent()
```


يحصل على قيمة تشير إلى ما إذا كان يجب زيادة ارتفاع الصف ليتناسب مع محتواه.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب زيادة ارتفاع الصف ليتناسب مع محتواه.
### getGridlines() {#getGridlines--}
```
public final List<Gridline> getGridlines()
```


يحصل على قائمة بـ [Gridline](../../com.aspose.tasks/gridline) التي تظهر في عرض المشروع.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridline&gt; - قائمة [Gridline](../../com.aspose.tasks/gridline) التي تظهر في منظور المشروع.
### getLegendDrawingOptions() {#getLegendDrawingOptions--}
```
public final int getLegendDrawingOptions()
```


يحصل على قيمة تحدد كيفية عرض وسيلة الإيضاح. القيمة الافتراضية هي LegendDrawingOptions.OnEveryPage.

ينطبق فقط عندما يتم عرض منظور مخطط جانت.

**Returns:**
int - قيمة تحدد كيفية عرض وسيلة الإيضاح.
### getLegendItems() {#getLegendItems--}
```
public final PageLegendItem[] getLegendItems()
```


يحصل على مصفوفة من PageLegendItem التي تحدد أي الأشرطة يجب عرضها في وسيلة إيضاح الصفحة. إذا كانت null، يتم عرض العناصر الافتراضية.

ينطبق فقط عندما يتم عرض منظور مخطط جانت.

**Returns:**
com.aspose.tasks.PageLegendItem[] - مصفوفة من PageLegendItem التي تحدد أي الأشرطة يجب عرضها في وسيلة إيضاح الصفحة.
### getMarkCriticalTasks() {#getMarkCriticalTasks--}
```
public final boolean getMarkCriticalTasks()
```


يحصل على قيمة تشير إلى ما إذا كان يجب عرض المهام الحرجة باللون الأحمر (القيمة الافتراضية هي FALSE).

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب عرض المهام الحرجة باللون الأحمر (القيمة الافتراضية هي FALSE).
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


يحصل على لون الوقت غير العامل.

**Returns:**
java.awt.Color - لون الوقت غير العامل.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


يحصل على عدد صفحات المشروع.

**Returns:**
int - عدد صفحات المشروع.
### getPageSize() {#getPageSize--}
```
public final int getPageSize()
```


يحصل على حجم الصفحة التي سيتم عرضها (القيمة الافتراضية هي PageSize.A4).

**Returns:**
int - حجم الصفحة التي سيتم عرضها (القيمة الافتراضية هي PageSize.A4).
### getPresentationFormat() {#getPresentationFormat--}
```
public final int getPresentationFormat()
```


يحصل على `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) التي سيتم حفظ المستند بها.

**Returns:**
int - الـ `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) الذي سيتم حفظ المستند به.
### getRenderToSinglePage() {#getRenderToSinglePage--}
```
public final boolean getRenderToSinglePage()
```


يحصل على قيمة تشير إلى ما إذا كان يجب عرض المشروع في صفحة واحدة عندما يتم حفظ المشروع بتنسيق رسومي. سيتم تغيير حجم الصفحة بحيث يمكن أن يتناسب المشروع المعروض على صفحة واحدة.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب عرض المشروع في صفحة واحدة عند حفظ المشروع بتنسيق رسومي.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


يحصل على قيمة تشير إلى ما إذا كان يجب وضع علامة على المهام الفرعية في شريط المهمة الملخصة. بالنسبة للمهام الفرعية، يشير حقل Rollup إلى ما إذا كانت المعلومات على أشرطة جانت للمهام الفرعية سيتم تجميعها إلى شريط المهمة الملخصة. بالنسبة للمهام الملخصة، يشير حقل Rollup إلى ما إذا كان شريط المهمة الملخصة يعرض أشرطة مجمعة. يجب أن يكون حقل Rollup للمهام الملخصة مضبوطًا على نعم لأي مهام فرعية لتجميعها إليها.

--------------------

ينطبق فقط عندما يتم عرض منظور مخطط جانت.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب وضع علامة على المهام الفرعية في شريط المهمة الملخصة.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


يحصل على التاريخ الذي يبدأ منه العرض.

**Returns:**
java.util.Date - التاريخ الذي يبدأ منه العرض.
### getTaskLinkDrawingCallback() {#getTaskLinkDrawingCallback--}
```
public final TaskLinkDrawingCallbackDelegate getTaskLinkDrawingCallback()
```


يحصل على رد نداء يمكن استخدامه لتخصيص بعض جوانب عرض روابط المهام.

ينطبق فقط عندما يتم عرض منظور مخطط جانت.

**Returns:**
[TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) - a callback that can be used to customize some aspects of task links rendering.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


يحصل على قائمة أنماط النص التي تُطبق أثناء عرض منظور المشروع.

--------------------

هذه الأنماط تتجاوز الأنماط المعرفة باستخدام GanttCharView.setTextStyles.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - قائمة أنماط النص التي تُطبق أثناء عرض رؤية المشروع.
### getTimescale() {#getTimescale--}
```
public final int getTimescale()
```


يحصل على قيمة `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) التي تُستخدم للتحكم في كيفية عرض المقياس الزمني (إن وجد) عندما يتم حفظ المشروع بتنسيق رسومي.

**Returns:**
int - قيمة `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) التي تُستخدم للتحكم في كيفية عرض مقياس الوقت (إن وجد) عندما يتم حفظ المشروع بتنسيق رسومي.
### getTimescaleFitBehavior() {#getTimescaleFitBehavior--}
```
public final int getTimescaleFitBehavior()
```


يحصل على سلوك يحدد كيفية محاذاة الطرف الأيمن للمقياس الزمني مع نهاية الصفحة.

**Returns:**
int - سلوك يحدد كيفية محاذاة الطرف الأيمن لمقياس الوقت مع نهاية الصفحة.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


يحصل على قيمة تشير إلى ما إذا كان يجب استخدام فرشاة التدرج عند عرض مخطط جانت.

--------------------

ينطبق فقط عندما يتم عرض منظور مخطط جانت.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب استخدام فرشاة التدرج عند عرض مخطط جانت.
### getView() {#getView--}
```
public final ProjectView getView()
```


يحصل على قائمة بأعمدة العرض التي سيتم عرضها ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). إذا لم يتم تعيينها فسيتم عرض معرفات المهام، أسماء المهام، البداية والنهاية فقط. إذا تم تعيين كل من خاصيتي View و `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-))، فإن الأعمدة من View تتجاوز الأعمدة من ViewSettings.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)).
### getViewSettings() {#getViewSettings--}
```
public final View getViewSettings()
```


يحصل على عرض (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) لعرضه. يمكنك استخدام هذه الخيارات لتحديد بشكل صريح أي عرض يجب حفظه بصيغ PDF أو HTML أو Image. إذا تم تعيين هذه الخاصية، يتم تجاهل خاصية [PresentationFormat](../../com.aspose.tasks/presentationformat) عند حفظ المشروع. يجب أن يكون العرض من إحدى الشاشات التالية ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Returns:**
[View](../../com.aspose.tasks/view) - a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


يحصل على قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا؛ يعيد false إذا كان اتجاه الصفحة أفقيًا.

--------------------

غير قابل للتطبيق عندما SaveOptions.getPageSize() == PageSize.DefinedInView. في هذه الحالة يتم استخدام [PageSettings.isPortrait()](../../com.aspose.tasks/pagesettings\#isPortrait--) بدلاً من ذلك. غير قابل للتطبيق عندما يتم تعيين [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--).

**Returns:**
boolean - قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا؛ تُعيد false إذا كان اتجاه الصفحة أفقيًا.
### setBarStyles(List&lt;BarStyle&gt; value) {#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--}
```
public final void setBarStyles(List<BarStyle> value)
```


يضبط قائمة مثيلات الفئة [BarStyle](../../com.aspose.tasks/barstyle) التي تظهر في منظور المشروع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.BarStyle&gt; | قائمة مثيلات الفئة [BarStyle](../../com.aspose.tasks/barstyle) التي تظهر في عرض المشروع. |

### setCustomPageSize(Dimension2D value) {#setCustomPageSize-java.awt.geom.Dimension2D-}
```
public final void setCustomPageSize(Dimension2D value)
```


يضبط حجم الصفحة المخصص بالنقاط (نقطة واحدة = 1/72 بوصة).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.geom.Dimension2D | حجم الصفحة المخصص بالنقاط (1 نقطة = 1/72 من البوصة). |

### setDrawNonWorkingTime(boolean value) {#setDrawNonWorkingTime-boolean-}
```
public final void setDrawNonWorkingTime(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب رسم وقت غير العمل (القيمة الافتراضية هي TRUE).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب رسم الوقت غير العامل (القيمة الافتراضية هي TRUE). |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


يضبط تاريخ الانتهاء من العرض.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | تاريخ لإنهاء العرض عنده. |

### setFitContent(boolean value) {#setFitContent-boolean-}
```
public final void setFitContent(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب زيادة ارتفاع الصف ليتناسب مع محتواه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب زيادة ارتفاع الصف ليتناسب مع محتواه. |

### setGridlines(List&lt;Gridline&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridline--}
```
public final void setGridlines(List<Gridline> value)
```


يضبط قائمة [Gridline](../../com.aspose.tasks/gridline) التي تظهر في منظور المشروع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridline&gt; | قائمة [Gridline](../../com.aspose.tasks/gridline) التي تظهر في عرض المشروع. |

### setLegendDrawingOptions(int value) {#setLegendDrawingOptions-int-}
```
public final void setLegendDrawingOptions(int value)
```


يضبط قيمة تحدد كيفية عرض المفتاح. القيمة الافتراضية هي LegendDrawingOptions.OnEveryPage.

ينطبق فقط عندما يتم عرض منظور مخطط جانت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة تحدد كيفية عرض المفتاح. |

### setLegendItems(PageLegendItem[] value) {#setLegendItems-com.aspose.tasks.PageLegendItem---}
```
public final void setLegendItems(PageLegendItem[] value)
```


يضبط مصفوفة من PageLegendItem التي تحدد أي الأشرطة يجب عرضها في مفتاح الصفحة. إذا كان null، يتم عرض العناصر الافتراضية.

ينطبق فقط عندما يتم عرض منظور مخطط جانت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [PageLegendItem\[\]](../../com.aspose.tasks/pagelegenditem) | مصفوفة من PageLegendItem التي تحدد أي الأشرطة يجب عرضها في مفتاح الصفحة. |

### setMarkCriticalTasks(boolean value) {#setMarkCriticalTasks-boolean-}
```
public final void setMarkCriticalTasks(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب عرض المهام الحرجة باللون الأحمر (القيمة الافتراضية هي FALSE).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب عرض المهام الحرجة باللون الأحمر (القيمة الافتراضية هي FALSE). |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


يضبط لون وقت غير العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color | لون وقت عدم العمل. |

### setPageSize(int value) {#setPageSize-int-}
```
public final void setPageSize(int value)
```


يضبط حجم الصفحة التي سيتم عرضها (القيمة الافتراضية هي PageSize.A4).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | حجم الصفحة التي سيتم عرضها (القيمة الافتراضية هي PageSize.A4). |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا؛ يعيد false إذا كان اتجاه الصفحة أفقيًا.

--------------------

غير قابل للتطبيق عندما SaveOptions.PageSize == Visualization.PageSize.DefinedInView. في هذه الحالة يتم استخدام [PageSettings.setPortrait(boolean)](../../com.aspose.tasks/pagesettings\#setPortrait-boolean-) بدلاً من ذلك. غير قابل للتطبيق عندما يتم تعيين [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا؛ تُعيد false إذا كان اتجاه الصفحة أفقيًا. |

### setPresentationFormat(int value) {#setPresentationFormat-int-}
```
public final void setPresentationFormat(int value)
```


يضبط `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) التي سيتم حفظ المستند بها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | int | الـ `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) الذي سيتم حفظ المستند به. |

### setRenderToSinglePage(boolean value) {#setRenderToSinglePage-boolean-}
```
public final void setRenderToSinglePage(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب عرض المشروع في صفحة واحدة عندما يتم حفظ المشروع بتنسيق رسومي. سيتم تغيير حجم الصفحة بحيث يمكن أن يتناسب المشروع المعروض في صفحة واحدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب عرض المشروع في صفحة واحدة عندما يتم حفظ المشروع بتنسيق رسومي. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب وضع علامة على المهام الفرعية في شريط المهمة الملخصة. بالنسبة للمهام الفرعية، يشير حقل Rollup إلى ما إذا كانت معلومات أشرطة جانت للمهام الفرعية ستُدمج في شريط المهمة الملخصة. بالنسبة للمهام الملخصة، يشير حقل Rollup إلى ما إذا كان شريط المهمة الملخصة يعرض أشرطة مدمجة. يجب أن يكون حقل Rollup للمهام الملخصة مضبوطًا على نعم لكي يتم دمج أي مهام فرعية فيها.

--------------------

ينطبق فقط عندما يتم عرض منظور مخطط جانت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب وضع علامة على المهام الفرعية في شريط المهمة الملخصة. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


يضبط التاريخ للبدء في العرض من.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | التاريخ للبدء في العرض منه. |

### setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value) {#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-}
```
public final void setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)
```


يضبط رد نداء يمكن استخدامه لتخصيص بعض جوانب عرض روابط المهام.

ينطبق فقط عندما يتم عرض منظور مخطط جانت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) | دالة رد نداء يمكن استخدامها لتخصيص بعض جوانب عرض روابط المهام. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


يضبط قائمة أنماط النص التي تُطبق أثناء عرض منظور المشروع.

--------------------

هذه الأنماط تتجاوز الأنماط المعرفة باستخدام GanttCharView.setTextStyles.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | قائمة أنماط النص التي تُطبق أثناء عرض منظور المشروع. |

### setTimescale(int value) {#setTimescale-int-}
```
public final void setTimescale(int value)
```


يضبط قيمة `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) التي تُستخدم للتحكم في كيفية عرض المقياس الزمني (إن وجد) عند حفظ المشروع بتنسيق رسومي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | int | قيمة `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) التي تُستخدم للتحكم في كيفية عرض مقياس الوقت (إن وجد) عندما يتم حفظ المشروع بتنسيق رسومي. |

### setTimescaleFitBehavior(int value) {#setTimescaleFitBehavior-int-}
```
public final void setTimescaleFitBehavior(int value)
```


يضبط سلوكًا يحدد كيفية محاذاة الطرف الأيمن للمقياس الزمني مع نهاية الصفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | سلوك يحدد كيفية محاذاة الطرف الأيمن لمقياس الوقت مع نهاية الصفحة. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب استخدام فرشاة التدرج عند عرض مخطط جانت.

--------------------

ينطبق فقط عندما يتم عرض منظور مخطط جانت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب استخدام فرشاة تدرجية عند عرض مخطط جانت. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


يضبط قائمة بأعمدة العرض التي سيتم عرضها ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). إذا لم يتم الضبط، فسيتم عرض معرفات المهام، أسماء المهام، البداية والنهاية فقط. إذا تم ضبط كل من View و `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-))، فإن الأعمدة من View تتجاوز الأعمدة من ViewSettings.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | قائمة بأعمدة العرض التي سيتم عرضها ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |

### setViewSettings(View value) {#setViewSettings-com.aspose.tasks.View-}
```
public final void setViewSettings(View value)
```


يضبط عرضًا (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) للعرض. يمكنك استخدام هذا الخيار لتحديد بشكل صريح أي عرض يجب حفظه بصيغ PDF أو HTML أو Image. إذا تم ضبط هذه الخاصية، يتم تجاهل خاصية [PresentationFormat](../../com.aspose.tasks/presentationformat) عند حفظ المشروع. يجب أن يكون العرض من إحدى الشاشات التالية ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | عرض (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) للعرض. |

