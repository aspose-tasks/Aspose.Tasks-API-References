---
title: "GanttBarStyle"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل نمط شريط يستخدمه MSP في عرض مخطط جانت."
type: docs
weight: 109
url: /ar/java/com.aspose.tasks/ganttbarstyle/
---

**Inheritance:**
java.lang.Object
```
public class GanttBarStyle
```

يمثل نمط شريط يستخدمه MSP في عرض مخطط جانت.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GanttBarStyle()](#GanttBarStyle--) | ينشئ مثلاً جديداً من فئة [GanttBarStyle](../../com.aspose/tasks/ganttbarstyle). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getBottomBarTextConverter()](#getBottomBarTextConverter--) | يحصل على محول معرف من قبل المستخدم للحصول على النص لعرضه في أسفل شريط المهمة. |
| [getBottomField()](#getBottomField--) | يحصل على البيانات التي ستُعرض في أسفل الشريط. |
| [getEndShape()](#getEndShape--) | يحصل على الشكل النهائي للشريط. |
| [getEndShapeColor()](#getEndShapeColor--) | يحصل على لون الشكل النهائي. |
| [getEndShapeType()](#getEndShapeType--) | يحصل على نوع الشكل النهائي. |
| [getFrom()](#getFrom--) | يحصل على موضع نقطة البداية لشريط الجانت. |
| [getInsideBarTextConverter()](#getInsideBarTextConverter--) | يحصل على محول معرف من قبل المستخدم للحصول على النص لعرضه داخل شريط المهمة. |
| [getInsideField()](#getInsideField--) | يحصل على البيانات التي ستُعرض داخل الشريط. |
| [getLeftBarTextConverter()](#getLeftBarTextConverter--) | يحصل على محول معرف من قبل المستخدم للحصول على النص لعرضه على يسار شريط المهمة. |
| [getLeftField()](#getLeftField--) | يحصل على البيانات التي ستُعرض على يسار الشريط. |
| [getMiddleFillPattern()](#getMiddleFillPattern--) | يحصل على نمط التعبئة لشريط الجانت. |
| [getMiddleShape()](#getMiddleShape--) | يحصل على الشكل الأوسط للشريط. |
| [getMiddleShapeColor()](#getMiddleShapeColor--) | يحصل على لون الشكل الأوسط. |
| [getName()](#getName--) | يحصل على اسم النمط. |
| [getParentStyle()](#getParentStyle--) | يحصل على النمط الأب (أو المشترك) للنمط المخصص الخاص بالمهمة. |
| [getRightBarTextConverter()](#getRightBarTextConverter--) | يحصل على محول معرف من قبل المستخدم للحصول على النص لعرضه على يمين شريط المهمة. |
| [getRightField()](#getRightField--) | يحصل على البيانات التي ستُعرض على يمين الشريط. |
| [getRow()](#getRow--) | يحصل على رقم الصف. |
| [getShowForCategories()](#getShowForCategories--) | يحصل على فئات المهمة التي يُطبق عليها النمط. |
| [getShowForTaskUid()](#getShowForTaskUid--) | يحصل على المعرف الفريد للمهمة التي يُطبق عليها النمط. |
| [getStartShape()](#getStartShape--) | يحصل على الشكل الابتدائي للشريط. |
| [getStartShapeColor()](#getStartShapeColor--) | يحصل على لون الشكل الابتدائي. |
| [getStartShapeType()](#getStartShapeType--) | يحصل على نوع الشكل الابتدائي. |
| [getTo()](#getTo--) | يحصل على موضع نقطة النهاية لشريط جانت. |
| [getTopBarTextConverter()](#getTopBarTextConverter--) | يحصل على محول معرف من قبل المستخدم للحصول على النص لعرضه أعلى شريط المهمة. |
| [getTopField()](#getTopField--) | يحصل على البيانات التي ستُعرض أعلى الشريط. |
| [setBottomBarTextConverter(TaskBarTextConverter value)](#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | يضبط محول معرف من قبل المستخدم للحصول على النص لعرضه أسفل شريط المهمة. |
| [setBottomField(int value)](#setBottomField-int-) | يضبط البيانات التي ستُعرض أسفل الشريط. |
| [setEndShape(int value)](#setEndShape-int-) | يضبط الشكل النهائي للشريط. |
| [setEndShapeColor(Color value)](#setEndShapeColor-java.awt.Color-) | يضبط لون الشكل النهائي. |
| [setEndShapeType(int value)](#setEndShapeType-int-) | يضبط نوع الشكل النهائي. |
| [setFrom(int value)](#setFrom-int-) | يضبط موضع نقطة البداية لشريط جانت. |
| [setInsideBarTextConverter(TaskBarTextConverter value)](#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | يضبط محول معرف من قبل المستخدم للحصول على النص لعرضه داخل شريط المهمة. |
| [setInsideField(int value)](#setInsideField-int-) | يضبط البيانات التي ستُعرض داخل الشريط. |
| [setLeftBarTextConverter(TaskBarTextConverter value)](#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | يضبط محول معرف من قبل المستخدم للحصول على النص لعرضه على يسار شريط المهمة. |
| [setLeftField(int value)](#setLeftField-int-) | يضبط البيانات التي ستُعرض على يسار الشريط. |
| [setMiddleFillPattern(int value)](#setMiddleFillPattern-int-) | يضبط نمط التعبئة لشريط جانت. |
| [setMiddleShape(int value)](#setMiddleShape-int-) | يضبط الشكل الأوسط للعمود. |
| [setMiddleShapeColor(Color value)](#setMiddleShapeColor-java.awt.Color-) | يضبط لون الشكل الأوسط. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم النمط. |
| [setParentStyle(GanttBarStyle value)](#setParentStyle-com.aspose.tasks.GanttBarStyle-) | يضبط النمط الأب (أو المشترك) للنمط المخصص الخاص بالمهمة. |
| [setRightBarTextConverter(TaskBarTextConverter value)](#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | يضبط المحول المعرّف من قبل المستخدم للحصول على النص ليتم عرضه على يمين شريط المهمة. |
| [setRightField(int value)](#setRightField-int-) | يضبط البيانات التي ستُعرض على يمين الشريط. |
| [setRow(int value)](#setRow-int-) | يضبط رقم الصف. |
| [setShowForCategories(List&lt;Integer&gt; value)](#setShowForCategories-java.util.List-java.lang.Integer--) | يضبط فئات المهام التي يُطبق عليها النمط. |
| [setShowForTaskUid(Integer value)](#setShowForTaskUid-java.lang.Integer-) | يضبط المعرف الفريد للمهمة التي يُطبق عليها النمط. |
| [setStartShape(int value)](#setStartShape-int-) | يضبط الشكل الابتدائي للعمود. |
| [setStartShapeColor(Color value)](#setStartShapeColor-java.awt.Color-) | يضبط لون الشكل الابتدائي. |
| [setStartShapeType(int value)](#setStartShapeType-int-) | يضبط نوع الشكل الابتدائي. |
| [setTo(int value)](#setTo-int-) | يضبط موضع نقطة النهاية لشريط جانت. |
| [setTopBarTextConverter(TaskBarTextConverter value)](#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | يضبط المحول المعرّف من قبل المستخدم للحصول على النص ليتم عرضه على أعلى شريط المهمة. |
| [setTopField(int value)](#setTopField-int-) | يضبط البيانات التي ستُعرض على أعلى الشريط. |
### GanttBarStyle() {#GanttBarStyle--}
```
public GanttBarStyle()
```


ينشئ مثلاً جديداً من فئة [GanttBarStyle](../../com.aspose/tasks/ganttbarstyle).

### getBottomBarTextConverter() {#getBottomBarTextConverter--}
```
public final TaskBarTextConverter getBottomBarTextConverter()
```


يحصل على المحول المعرّف من قبل المستخدم للحصول على النص ليتم عرضه على أسفل شريط المهمة. يتجاوز قيمة الخاصية `BottomField`([getBottomField()](../../com.aspose.tasks/ganttbarstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/ganttbarstyle\#setBottomField-int-)).

--------------------

لا يتم حفظه إلى تنسيق MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the bottom of the task's bar.
### getBottomField() {#getBottomField--}
```
public final int getBottomField()
```


يحصل على البيانات التي ستُعرض على أسفل الشريط. [Field](../../com.aspose.tasks/field).

**Returns:**
int - البيانات التي ستُعرض على أسفل الشريط.
### getEndShape() {#getEndShape--}
```
public final int getEndShape()
```


يحصل على الشكل النهائي للشريط.

**Returns:**
int - شكل النهاية للعمود.
### getEndShapeColor() {#getEndShapeColor--}
```
public final Color getEndShapeColor()
```


يحصل على لون الشكل النهائي.

**Returns:**
java.awt.Color - لون شكل النهاية.
### getEndShapeType() {#getEndShapeType--}
```
public final int getEndShapeType()
```


يحصل على نوع شكل النهاية. [GanttBarType](../../com.aspose.tasks/ganttbartype).

**Returns:**
int - نوع شكل النهاية.
### getFrom() {#getFrom--}
```
public final int getFrom()
```


يحصل على موضع نقطة البداية لشريط جانت. [Field](../../com.aspose.tasks/field).

**Returns:**
int - موضع نقطة البداية لشريط جانت.
### getInsideBarTextConverter() {#getInsideBarTextConverter--}
```
public final TaskBarTextConverter getInsideBarTextConverter()
```


يسترجع محولًا معرفًا من قبل المستخدم للحصول على النص لتصميمه داخل شريط المهمة. يتجاوز قيمة `InsideField`([getInsideField()](../../com.aspose/tasks/ganttbarstyle\\#getInsideField--)/[setInsideField(int)](../../com.aspose/tasks/ganttbarstyle\\#setInsideField-int-)) الخاصية.

--------------------

لا يتم حفظه إلى تنسيق MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render inside of the task's bar.
### getInsideField() {#getInsideField--}
```
public final int getInsideField()
```


يسترجع البيانات التي سيتم عرضها داخل الشريط. [Field](../../com.aspose/tasks/field).

**Returns:**
int - البيانات التي سيتم عرضها داخل الشريط.
### getLeftBarTextConverter() {#getLeftBarTextConverter--}
```
public final TaskBarTextConverter getLeftBarTextConverter()
```


يسترجع محولًا معرفًا من قبل المستخدم للحصول على النص لتصميمه على يسار شريط المهمة. يتجاوز قيمة `LeftField`([getLeftField()](../../com.aspose/tasks/ganttbarstyle\\#getLeftField--)/[setLeftField(int)](../../com.aspose/tasks/ganttbarstyle\\#setLeftField-int-)) الخاصية.

--------------------

لا يتم حفظه إلى تنسيق MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the left of the task's bar.
### getLeftField() {#getLeftField--}
```
public final int getLeftField()
```


يسترجع البيانات التي سيتم عرضها على يسار الشريط. [Field](../../com.aspose/tasks/field).

**Returns:**
int - البيانات التي سيتم عرضها على يسار الشريط.
### getMiddleFillPattern() {#getMiddleFillPattern--}
```
public final int getMiddleFillPattern()
```


يحصل على نمط التعبئة لشريط الجانت.

**Returns:**
int - نمط تعبئة شريط جانت.
### getMiddleShape() {#getMiddleShape--}
```
public final int getMiddleShape()
```


يحصل على الشكل الأوسط للشريط.

**Returns:**
int - شكل متوسط للشريط.
### getMiddleShapeColor() {#getMiddleShapeColor--}
```
public final Color getMiddleShapeColor()
```


يحصل على لون الشكل الأوسط.

**Returns:**
java.awt.Color - لون الشكل المتوسط.
### getName() {#getName--}
```
public final String getName()
```


يحصل على اسم النمط.

**Returns:**
java.lang.String - اسم النمط.
### getParentStyle() {#getParentStyle--}
```
public final GanttBarStyle getParentStyle()
```


يحصل على النمط الأب (أو المشترك) للنمط المخصص الخاص بالمهمة.

--------------------

يمكن للمهمة أن تحتوي على أنماط مخصصة متعددة مع أنماط أصلية مختلفة. على سبيل المثال، اعتبر مهمة لها نمط مخصص مع نمط أصل \"Critical\" ونمط آخر مع نمط أصل \"Normal\". ببساطة، إذا كانت المهمة حرجة، يُطبق النمط الأول. إذا أصبحت غير حرجة، يُطبق النمط الثاني (هذا المنطق مستمد من Microsoft Project Professional).

**Returns:**
[GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) - parent (or common) style for custom task-specific style.
### getRightBarTextConverter() {#getRightBarTextConverter--}
```
public final TaskBarTextConverter getRightBarTextConverter()
```


يسترجع محولًا معرفًا من قبل المستخدم للحصول على النص لتصميمه على يمين شريط المهمة. يتجاوز قيمة `RightField`([getRightField()](../../com.aspose/tasks/ganttbarstyle\\#getRightField--)/[setRightField(int)](../../com.aspose/tasks/ganttbarstyle\\#setRightField-int-)) الخاصية.

--------------------

لا يتم حفظه إلى تنسيق MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the right of the task's bar.
### getRightField() {#getRightField--}
```
public final int getRightField()
```


يسترجع البيانات التي سيتم عرضها على يمين الشريط. [Field](../../com.aspose/tasks/field).

**Returns:**
int - البيانات التي سيتم عرضها على يمين الشريط.
### getRow() {#getRow--}
```
public final int getRow()
```


يحصل على رقم الصف.

--------------------

يمكن أن تكون من 1 إلى 4 (1 هي القيمة الافتراضية).

**Returns:**
int - رقم الصف.
### getShowForCategories() {#getShowForCategories--}
```
public final List<Integer> getShowForCategories()
```


يسترجع فئات المهام التي يُطبق عليها النمط. ينطبق على الأنماط الأصلية (أو المشتركة) لأشرطة مخطط جانت (انظر `GanttChartView.BarStyles`([GanttChartView.getBarStyles()](../../com.aspose/tasks/ganttchartview\\#getBarStyles--))).

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - فئات المهام التي يُطبق عليها النمط.
### getShowForTaskUid() {#getShowForTaskUid--}
```
public final Integer getShowForTaskUid()
```


يسترجع المعرف الفريد لمهمة يُطبق عليها النمط. ينطبق على الأنماط الخاصة بالمهمة لأشرطة مخطط جانت (انظر `GanttChartView.CustomBarStyles`([GanttChartView.getCustomBarStyles()](../../com.aspose/tasks/ganttchartview\\#getCustomBarStyles--))).

**Returns:**
java.lang.Integer - المعرف الفريد لمهمة يُطبق عليها النمط.
### getStartShape() {#getStartShape--}
```
public final int getStartShape()
```


يحصل على الشكل الابتدائي للشريط.

**Returns:**
int - شكل البداية للشريط.
### getStartShapeColor() {#getStartShapeColor--}
```
public final Color getStartShapeColor()
```


يحصل على لون الشكل الابتدائي.

**Returns:**
java.awt.Color - لون شكل البداية.
### getStartShapeType() {#getStartShapeType--}
```
public final int getStartShapeType()
```


يحصل على نوع الشكل الابتدائي.

**Returns:**
int - نوع شكل البداية.
### getTo() {#getTo--}
```
public final int getTo()
```


يحصل على موضع نقطة النهاية لشريط جانت.

**Returns:**
int - موضع نقطة النهاية لشريط جانت.
### getTopBarTextConverter() {#getTopBarTextConverter--}
```
public final TaskBarTextConverter getTopBarTextConverter()
```


يسترجع محولًا معرفًا من قبل المستخدم للحصول على النص لتصميمه على أعلى شريط المهمة. يتجاوز قيمة `TopField`([getTopField()](../../com.aspose/tasks/ganttbarstyle\\#getTopField--)/[setTopField(int)](../../com.aspose/tasks/ganttbarstyle\\#setTopField-int-)) الخاصية.

--------------------

لا يتم حفظه إلى تنسيق MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the top of the task's bar.
### getTopField() {#getTopField--}
```
public final int getTopField()
```


يحصل على البيانات التي ستُعرض أعلى الشريط.

**Returns:**
int - البيانات التي سيتم عرضها في أعلى الشريط.
### setBottomBarTextConverter(TaskBarTextConverter value) {#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setBottomBarTextConverter(TaskBarTextConverter value)
```


يضبط المحول المعرّف من قبل المستخدم للحصول على النص لتصميمه في أسفل شريط المهمة. يتجاوز قيمة `BottomField`([getBottomField()](../../com.aspose.tasks/ganttbarstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/ganttbarstyle\#setBottomField-int-)) الخاصية.

--------------------

لا يتم حفظه إلى تنسيق MPP.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | محول معرف من قبل المستخدم للحصول على النص لتصميمه في أسفل شريط المهمة. |

### setBottomField(int value) {#setBottomField-int-}
```
public final void setBottomField(int value)
```


يضبط البيانات التي سيتم عرضها في أسفل الشريط. [Field](../../com.aspose.tasks/field).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | البيانات التي سيتم عرضها في أسفل الشريط. |

### setEndShape(int value) {#setEndShape-int-}
```
public final void setEndShape(int value)
```


يضبط الشكل النهائي للشريط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | شكل نهائي للشريط. |

### setEndShapeColor(Color value) {#setEndShapeColor-java.awt.Color-}
```
public final void setEndShapeColor(Color value)
```


يضبط لون الشكل النهائي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color | لون الشكل النهائي. |

### setEndShapeType(int value) {#setEndShapeType-int-}
```
public final void setEndShapeType(int value)
```


يضبط نوع الشكل النهائي. [GanttBarType](../../com.aspose.tasks/ganttbartype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نوع الشكل النهائي. |

### setFrom(int value) {#setFrom-int-}
```
public final void setFrom(int value)
```


يضبط موضع نقطة البداية لشريط جانت. [Field](../../com.aspose.tasks/field).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | موضع نقطة البداية لشريط جانت. |

### setInsideBarTextConverter(TaskBarTextConverter value) {#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setInsideBarTextConverter(TaskBarTextConverter value)
```


يضبط المحول المعرّف من قبل المستخدم للحصول على النص لتصميمه داخل شريط المهمة. يتجاوز قيمة `InsideField`([getInsideField()](../../com.aspose.tasks/ganttbarstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose.tasks/ganttbarstyle\#setInsideField-int-)) الخاصية.

--------------------

لا يتم حفظه إلى تنسيق MPP.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | محول معرف من قبل المستخدم للحصول على النص لتصميمه داخل شريط المهمة. |

### setInsideField(int value) {#setInsideField-int-}
```
public final void setInsideField(int value)
```


يضبط البيانات التي سيتم عرضها داخل الشريط. [Field](../../com.aspose.tasks/field).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | البيانات التي سيتم عرضها داخل الشريط. |

### setLeftBarTextConverter(TaskBarTextConverter value) {#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setLeftBarTextConverter(TaskBarTextConverter value)
```


يضبط المحول المعرّف من قبل المستخدم للحصول على النص لتصميمه على يسار شريط المهمة. يتجاوز قيمة `LeftField`([getLeftField()](../../com.aspose.tasks/ganttbarstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose.tasks/ganttbarstyle\#setLeftField-int-)) الخاصية.

--------------------

لا يتم حفظه إلى تنسيق MPP.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | محول معرف من قبل المستخدم للحصول على النص لتصميمه على يسار شريط المهمة. |

### setLeftField(int value) {#setLeftField-int-}
```
public final void setLeftField(int value)
```


يضبط البيانات التي سيتم عرضها على يسار الشريط. [Field](../../com.aspose.tasks/field).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | البيانات التي سيتم عرضها على يسار الشريط. |

### setMiddleFillPattern(int value) {#setMiddleFillPattern-int-}
```
public final void setMiddleFillPattern(int value)
```


يضبط نمط التعبئة لشريط جانت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نمط تعبئة لشريط جانت. |

### setMiddleShape(int value) {#setMiddleShape-int-}
```
public final void setMiddleShape(int value)
```


يضبط الشكل الأوسط للعمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | شكل متوسط للشريط. |

### setMiddleShapeColor(Color value) {#setMiddleShapeColor-java.awt.Color-}
```
public final void setMiddleShapeColor(Color value)
```


يضبط لون الشكل الأوسط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color | لون الشكل المتوسط. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


يضبط اسم النمط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | اسم النمط. |

### setParentStyle(GanttBarStyle value) {#setParentStyle-com.aspose.tasks.GanttBarStyle-}
```
public final void setParentStyle(GanttBarStyle value)
```


يضبط النمط الأب (أو المشترك) للنمط المخصص الخاص بالمهمة.

--------------------

يمكن للمهمة أن تحتوي على أنماط مخصصة متعددة مع أنماط أصلية مختلفة. على سبيل المثال، اعتبر مهمة لها نمط مخصص مع نمط أصل \"Critical\" ونمط آخر مع نمط أصل \"Normal\". ببساطة، إذا كانت المهمة حرجة، يُطبق النمط الأول. إذا أصبحت غير حرجة، يُطبق النمط الثاني (هذا المنطق مستمد من Microsoft Project Professional).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) | النمط الأب (أو الشائع) للنمط المخصص الخاص بالمهمة. |

### setRightBarTextConverter(TaskBarTextConverter value) {#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setRightBarTextConverter(TaskBarTextConverter value)
```


يضبط المحول المعرّف من قبل المستخدم للحصول على النص لتصميمه على يمين شريط المهمة. يتجاوز قيمة `RightField`([getRightField()](../../com.aspose.tasks/ganttbarstyle\#getRightField--)/[setRightField(int)](../../com.aspose.tasks/ganttbarstyle\#setRightField-int-)) الخاصية.

--------------------

لا يتم حفظه إلى تنسيق MPP.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | محول معرف من قبل المستخدم للحصول على النص لتصميمه على يمين شريط المهمة. |

### setRightField(int value) {#setRightField-int-}
```
public final void setRightField(int value)
```


يضبط البيانات المعروضة على يمين الشريط. [Field](../../com.aspose.tasks/field).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | البيانات المعروضة على يمين الشريط. |

### setRow(int value) {#setRow-int-}
```
public final void setRow(int value)
```


يضبط رقم الصف.

--------------------

يمكن أن تكون من 1 إلى 4 (1 هي القيمة الافتراضية).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | رقم الصف. |

### setShowForCategories(List&lt;Integer&gt; value) {#setShowForCategories-java.util.List-java.lang.Integer--}
```
public final void setShowForCategories(List<Integer> value)
```


يضبط فئات المهام التي يتم تطبيق النمط عليها. ينطبق على الأنماط الأصلية (أو العامة) لأشرطة المخطط الزمني (انظر `GanttChartView.BarStyles`([GanttChartView.getBarStyles()](../../com.aspose.tasks/ganttchartview\#getBarStyles--))).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.List&lt;java.lang.Integer&gt; | فئات المهام التي يتم تطبيق النمط عليها. |

### setShowForTaskUid(Integer value) {#setShowForTaskUid-java.lang.Integer-}
```
public final void setShowForTaskUid(Integer value)
```


يضبط المعرف الفريد لمهمة يتم تطبيق النمط عليها. ينطبق على الأنماط الخاصة بالمهمة لأشرطة المخطط الزمني (انظر `GanttChartView.CustomBarStyles`([GanttChartView.getCustomBarStyles()](../../com.aspose.tasks/ganttchartview\#getCustomBarStyles--))).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Integer | المعرف الفريد لمهمة يتم تطبيق النمط عليها. |

### setStartShape(int value) {#setStartShape-int-}
```
public final void setStartShape(int value)
```


يضبط الشكل الابتدائي للعمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | شكل بداية الشريط. |

### setStartShapeColor(Color value) {#setStartShapeColor-java.awt.Color-}
```
public final void setStartShapeColor(Color value)
```


يضبط لون الشكل الابتدائي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color | لون شكل البداية. |

### setStartShapeType(int value) {#setStartShapeType-int-}
```
public final void setStartShapeType(int value)
```


يضبط نوع الشكل الابتدائي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نوع شكل البداية. |

### setTo(int value) {#setTo-int-}
```
public final void setTo(int value)
```


يضبط موضع نقطة النهاية لشريط جانت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | موضع نقطة النهاية لشريط المخطط الزمني. |

### setTopBarTextConverter(TaskBarTextConverter value) {#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setTopBarTextConverter(TaskBarTextConverter value)
```


يضبط محول معرف من قبل المستخدم للحصول على النص لتصميمه على أعلى شريط المهمة. يتجاوز قيمة الخاصية `TopField`([getTopField()](../../com.aspose.tasks/ganttbarstyle\#getTopField--)/[setTopField(int)](../../com.aspose.tasks/ganttbarstyle\#setTopField-int-)).

--------------------

لا يتم حفظه إلى تنسيق MPP.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | محول معرف من قبل المستخدم للحصول على النص لتصميمه على أعلى شريط المهمة. |

### setTopField(int value) {#setTopField-int-}
```
public final void setTopField(int value)
```


يضبط البيانات التي ستُعرض على أعلى الشريط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | البيانات المعروضة على أعلى الشريط. |

