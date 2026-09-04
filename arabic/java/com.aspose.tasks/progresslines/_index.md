---
title: "خطوط التقدم"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل خطوط التقدم في عرض مخطط جانت."
type: docs
weight: 219
url: /ar/java/com.aspose.tasks/progresslines/
---

**Inheritance:**
java.lang.Object
```
public class ProgressLines
```

يمثل خطوط التقدم في عرض مخطط جانت.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ProgressLines()](#ProgressLines--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getBeginAtDate()](#getBeginAtDate--) | يحصل على التاريخ لعرض خطوط التقدم منه. |
| [getBeginAtProjectStart()](#getBeginAtProjectStart--) | يحصل على قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم من بداية تاريخ بدء المشروع. |
| [getDateFormat()](#getDateFormat--) | يحصل على تنسيق التاريخ ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [getDisplayAtCurrentDate()](#getDisplayAtCurrentDate--) | يحصل على قيمة تشير إلى ما إذا كان سيتم عرض خط التقدم عند التاريخ الحالي. |
| [getDisplayAtRecurringIntervals()](#getDisplayAtRecurringIntervals--) | يحصل على قيمة تشير إلى ما إذا كان سيتم عرض خط التقدم على فترات متكررة. |
| [getDisplaySelected()](#getDisplaySelected--) | يحصل على قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم في التواريخ المحددة. |
| [getFont()](#getFont--) | يحصل على الخط المستخدم لتسمية خط التقدم. |
| [getLineColor()](#getLineColor--) | يحصل على لون الخط لخط التقدم الحالي. |
| [getLinePattern()](#getLinePattern--) | يحصل على نمط الخط لخط التقدم الحالي. |
| [getOtherLineColor()](#getOtherLineColor--) | يحصل على لون خط التقدم الآخر. |
| [getOtherLinePattern()](#getOtherLinePattern--) | يحصل على نمط الخط لخط التقدم الآخر. |
| [getOtherProgressPointColor()](#getOtherProgressPointColor--) | يحصل على لون نقطة التقدم الأخرى. |
| [getOtherProgressPointShape()](#getOtherProgressPointShape--) | يحصل على شكل نقطة التقدم لخط التقدم الآخر. |
| [getProgressPointColor()](#getProgressPointColor--) | يحصل على لون نقطة التقدم. |
| [getProgressPointShape()](#getProgressPointShape--) | يحصل على شكل نقطة التقدم. |
| [getRecurringInterval()](#getRecurringInterval--) | يحصل على الفاصل المتكرر. |
| [getSelectedDates()](#getSelectedDates--) | يحصل على قائمة التواريخ المحددة لعرض خطوط التقدم لها. |
| [getShowDate()](#getShowDate--) | يحصل على قيمة تشير إلى ما إذا كان سيتم إظهار التاريخ لكل خط تقدم. |
| [isBaselinePlan()](#isBaselinePlan--) | يحصل على قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم للخطة الأساسية أو الفعلية. |
| [isBaselinePlan(boolean value)](#isBaselinePlan-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم للخطة الأساسية أو الفعلية. |
| [setBeginAtDate(Date value)](#setBeginAtDate-java.util.Date-) | يضبط التاريخ لبدء عرض خطوط التقدم منه. |
| [setBeginAtProjectStart(boolean value)](#setBeginAtProjectStart-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم من بداية تاريخ بدء المشروع. |
| [setDateFormat(int value)](#setDateFormat-int-) | يضبط تنسيق التاريخ ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [setDisplayAtCurrentDate(boolean value)](#setDisplayAtCurrentDate-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم عرض خط التقدم عند التاريخ الحالي. |
| [setDisplayAtRecurringIntervals(boolean value)](#setDisplayAtRecurringIntervals-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم عرض خط التقدم على فترات متكررة. |
| [setDisplaySelected(boolean value)](#setDisplaySelected-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم في التواريخ المحددة. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | يضبط الخط المستخدم لتسمية خط التقدم. |
| [setLineColor(Color value)](#setLineColor-java.awt.Color-) | يضبط لون الخط لخط التقدم الحالي. |
| [setLinePattern(int value)](#setLinePattern-int-) | يضبط نمط الخط لخط التقدم الحالي. |
| [setOtherLineColor(Color value)](#setOtherLineColor-java.awt.Color-) | يضبط لون خط التقدم الآخر. |
| [setOtherLinePattern(int value)](#setOtherLinePattern-int-) | يضبط نمط الخط لخط التقدم الآخر. |
| [setOtherProgressPointColor(Color value)](#setOtherProgressPointColor-java.awt.Color-) | يضبط لون نقطة التقدم الأخرى. |
| [setOtherProgressPointShape(int value)](#setOtherProgressPointShape-int-) | يضبط شكل نقطة التقدم لخط التقدم الآخر. |
| [setProgressPointColor(Color value)](#setProgressPointColor-java.awt.Color-) | يضبط لون نقطة التقدم. |
| [setProgressPointShape(int value)](#setProgressPointShape-int-) | يضبط شكل نقطة التقدم. |
| [setRecurringInterval(RecurringInterval value)](#setRecurringInterval-com.aspose.tasks.RecurringInterval-) | يضبط الفاصل المتكرر. |
| [setShowDate(boolean value)](#setShowDate-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب إظهار التاريخ لكل خط تقدم. |
### ProgressLines() {#ProgressLines--}
```
public ProgressLines()
```


### getBeginAtDate() {#getBeginAtDate--}
```
public final Date getBeginAtDate()
```


يحصل على التاريخ لعرض خطوط التقدم منه.

**Returns:**
java.util.Date - التاريخ لعرض خطوط التقدم منه.
### getBeginAtProjectStart() {#getBeginAtProjectStart--}
```
public final boolean getBeginAtProjectStart()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم من بداية تاريخ بدء المشروع.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب عرض خطوط التقدم من بداية تاريخ بدء المشروع.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


يحصل على تنسيق التاريخ ([DateLabel](../../com.aspose.tasks/datelabel)).

**Returns:**
int - تنسيق التاريخ ([DateLabel](../../com.aspose.tasks/datelabel)).
### getDisplayAtCurrentDate() {#getDisplayAtCurrentDate--}
```
public final boolean getDisplayAtCurrentDate()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم عرض خط التقدم عند التاريخ الحالي.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب عرض خط التقدم في التاريخ الحالي.
### getDisplayAtRecurringIntervals() {#getDisplayAtRecurringIntervals--}
```
public final boolean getDisplayAtRecurringIntervals()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم عرض خط التقدم على فترات متكررة.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب عرض خط التقدم عند الفواصل المتكررة.
### getDisplaySelected() {#getDisplaySelected--}
```
public final boolean getDisplaySelected()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم في التواريخ المحددة.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب عرض خطوط التقدم في التواريخ المختارة.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


يحصل على الخط المستخدم لتسمية خط التقدم.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font used for progress line label.
### getLineColor() {#getLineColor--}
```
public final Color getLineColor()
```


يحصل على لون الخط لخط التقدم الحالي.

**Returns:**
java.awt.Color - لون الخط لخط التقدم الحالي.
### getLinePattern() {#getLinePattern--}
```
public final int getLinePattern()
```


يحصل على نمط الخط لخط التقدم الحالي. `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Returns:**
int - نمط الخط لخط التقدم الحالي.
### getOtherLineColor() {#getOtherLineColor--}
```
public final Color getOtherLineColor()
```


يحصل على لون خط التقدم الآخر.

**Returns:**
java.awt.Color - لون خط التقدم الآخر.
### getOtherLinePattern() {#getOtherLinePattern--}
```
public final int getOtherLinePattern()
```


يحصل على نمط الخط لخط التقدم الآخر.

**Returns:**
int - نمط الخط لخط التقدم الآخر.
### getOtherProgressPointColor() {#getOtherProgressPointColor--}
```
public final Color getOtherProgressPointColor()
```


يحصل على لون نقطة التقدم الأخرى.

**Returns:**
java.awt.Color - لون نقطة التقدم الأخرى.
### getOtherProgressPointShape() {#getOtherProgressPointShape--}
```
public final int getOtherProgressPointShape()
```


يحصل على شكل نقطة التقدم لخط التقدم الآخر.

**Returns:**
int - شكل نقطة التقدم لخط التقدم الآخر.
### getProgressPointColor() {#getProgressPointColor--}
```
public final Color getProgressPointColor()
```


يحصل على لون نقطة التقدم.

**Returns:**
java.awt.Color - لون نقطة التقدم.
### getProgressPointShape() {#getProgressPointShape--}
```
public final int getProgressPointShape()
```


يحصل على شكل نقطة التقدم. [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Returns:**
int - شكل نقطة التقدم.
### getRecurringInterval() {#getRecurringInterval--}
```
public final RecurringInterval getRecurringInterval()
```


يحصل على الفاصل المتكرر. `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Returns:**
[RecurringInterval](../../com.aspose.tasks/recurringinterval) - the recurring interval.
### getSelectedDates() {#getSelectedDates--}
```
public final List<Date> getSelectedDates()
```


يحصل على قائمة التواريخ المحددة لعرض خطوط التقدم لها.

**Returns:**
java.util.List&lt;java.util.Date&gt; - قائمة التواريخ المحددة لعرض خطوط التقدم لها.
### getShowDate() {#getShowDate--}
```
public final boolean getShowDate()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم إظهار التاريخ لكل خط تقدم.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب إظهار التاريخ لكل خط تقدم.
### isBaselinePlan() {#isBaselinePlan--}
```
public final boolean isBaselinePlan()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم للخطة الأساسية أو الفعلية.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب عرض خطوط التقدم للخطة الأساسية أو الفعلية.
### isBaselinePlan(boolean value) {#isBaselinePlan-boolean-}
```
public final void isBaselinePlan(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم للخطة الأساسية أو الفعلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب عرض خطوط التقدم للخطة الأساسية أو الفعلية. |

### setBeginAtDate(Date value) {#setBeginAtDate-java.util.Date-}
```
public final void setBeginAtDate(Date value)
```


يضبط التاريخ لبدء عرض خطوط التقدم منه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | التاريخ الذي تُعرض منه خطوط التقدم. |

### setBeginAtProjectStart(boolean value) {#setBeginAtProjectStart-boolean-}
```
public final void setBeginAtProjectStart(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم من بداية تاريخ بدء المشروع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب عرض خطوط التقدم من بداية تاريخ بدء المشروع. |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


يضبط تنسيق التاريخ ([DateLabel](../../com.aspose.tasks/datelabel)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | int | تنسيق التاريخ ([DateLabel](../../com.aspose.tasks/datelabel)). |

### setDisplayAtCurrentDate(boolean value) {#setDisplayAtCurrentDate-boolean-}
```
public final void setDisplayAtCurrentDate(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم عرض خط التقدم عند التاريخ الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب عرض خط التقدم في التاريخ الحالي. |

### setDisplayAtRecurringIntervals(boolean value) {#setDisplayAtRecurringIntervals-boolean-}
```
public final void setDisplayAtRecurringIntervals(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم عرض خط التقدم على فترات متكررة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب عرض خط التقدم على فواصل متكررة. |

### setDisplaySelected(boolean value) {#setDisplaySelected-boolean-}
```
public final void setDisplaySelected(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم في التواريخ المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب عرض خطوط التقدم في التواريخ المحددة. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


يضبط الخط المستخدم لتسمية خط التقدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | الخط المستخدم لتسمية خط التقدم. |

### setLineColor(Color value) {#setLineColor-java.awt.Color-}
```
public final void setLineColor(Color value)
```


يضبط لون الخط لخط التقدم الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color | لون الخط لخط التقدم الحالي. |

### setLinePattern(int value) {#setLinePattern-int-}
```
public final void setLinePattern(int value)
```


يضبط نمط الخط لخط التقدم الحالي. `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نمط الخط لخط التقدم الحالي. |

### setOtherLineColor(Color value) {#setOtherLineColor-java.awt.Color-}
```
public final void setOtherLineColor(Color value)
```


يضبط لون خط التقدم الآخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color | لون الخط لخط التقدم الآخر. |

### setOtherLinePattern(int value) {#setOtherLinePattern-int-}
```
public final void setOtherLinePattern(int value)
```


يضبط نمط الخط لخط التقدم الآخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نمط الخط لخط التقدم الآخر. |

### setOtherProgressPointColor(Color value) {#setOtherProgressPointColor-java.awt.Color-}
```
public final void setOtherProgressPointColor(Color value)
```


يضبط لون نقطة التقدم الأخرى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color | لون النقطة الأخرى للتقدم. |

### setOtherProgressPointShape(int value) {#setOtherProgressPointShape-int-}
```
public final void setOtherProgressPointShape(int value)
```


يضبط شكل نقطة التقدم لخط التقدم الآخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | شكل نقطة التقدم لخط التقدم الآخر. |

### setProgressPointColor(Color value) {#setProgressPointColor-java.awt.Color-}
```
public final void setProgressPointColor(Color value)
```


يضبط لون نقطة التقدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color | لون نقطة التقدم. |

### setProgressPointShape(int value) {#setProgressPointShape-int-}
```
public final void setProgressPointShape(int value)
```


يضبط شكل نقطة التقدم. [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | شكل نقطة التقدم. |

### setRecurringInterval(RecurringInterval value) {#setRecurringInterval-com.aspose.tasks.RecurringInterval-}
```
public final void setRecurringInterval(RecurringInterval value)
```


يضبط الفاصل المتكرر. `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [RecurringInterval](../../com.aspose.tasks/recurringinterval) | الفاصل المتكرر. |

### setShowDate(boolean value) {#setShowDate-boolean-}
```
public final void setShowDate(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب إظهار التاريخ لكل خط تقدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب عرض التاريخ لكل سطر تقدم. |

