---
title: "GroupCriterion"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل معيارًا في تعريف مجموعة."
type: docs
weight: 124
url: /ar/java/com.aspose.tasks/groupcriterion/
---

**Inheritance:**
java.lang.Object
```
public class GroupCriterion
```

يمثل معيارًا في تعريف مجموعة. كائن GroupCriterion هو عضو في مجموعة [GroupCriterionCollection](../../com.aspose.tasks/groupcriterioncollection).
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GroupCriterion()](#GroupCriterion--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [getAscending()](#getAscending--) | يحصل على قيمة تشير إلى ما إذا كان الحقل المستخدم كمعيار في تعريف مجموعة مُرتبًا تصاعديًا. |
| [getCellColor()](#getCellColor--) | يحصل على لون خلفية الخلية لحقل يُستخدم كمعيار في تعريف مجموعة. |
| [getField()](#getField--) | يحصل على الحقل الذي يتم تجميعه. |
| [getFont()](#getFont--) | يحصل على الخط للمعيار في تعريف مجموعة. |
| [getFontColor()](#getFontColor--) | يحصل على لون الخط للحقل المستخدم كمعيار في تعريف مجموعة. |
| [getGroupInterval()](#getGroupInterval--) | يحصل على الفاصل الزمني للحقل المستخدم كمعيار في تعريف مجموعة. |
| [getGroupOn()](#getGroupOn--) | يحصل على نوع التجميع للحقل المستخدم كمعيار في تعريف مجموعة. |
| [getPattern()](#getPattern--) | يحصل على نمط الخلية للحقل المستخدم كمعيار في تعريف مجموعة. |
| [getStartAt()](#getStartAt--) | يحصل على بداية الفواصل الزمنية للحقل المستخدم كمعيار في تعريف مجموعة. |
| [hashCode()](#hashCode--) | يعمل كدالة تجزئة لنوع معين. |
| [setAscending(boolean value)](#setAscending-boolean-) | يضبط قيمة تشير إلى ما إذا كان الحقل المستخدم كمعيار في تعريف المجموعة مُرتّبًا بترتيب تصاعدي. |
| [setCellColor(Color value)](#setCellColor-java.awt.Color-) | يضبط لون خلفية الخلية لحقل يُستخدم كمعيار في تعريف المجموعة. |
| [setField(int value)](#setField-int-) | يضبط الحقل الذي يتم التجميع بناءً عليه. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | يضبط الخط للمعيار في تعريف المجموعة. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | يضبط لون الخط للحقل المستخدم كمعيار في تعريف المجموعة. |
| [setGroupInterval(Object value)](#setGroupInterval-java.lang.Object-) | يضبط الفاصل الزمني للحقل المستخدم كمعيار في تعريف المجموعة. |
| [setGroupOn(int value)](#setGroupOn-int-) | يضبط نوع التجميع للحقل المستخدم كمعيار في تعريف المجموعة. |
| [setPattern(int value)](#setPattern-int-) | يضبط نمط الخلية للحقل المستخدم كمعيار في تعريف المجموعة. |
| [setStartAt(Object value)](#setStartAt-java.lang.Object-) | يضبط بداية الفواصل للحقل المستخدم كمعيار في تعريف المجموعة. |
### GroupCriterion() {#GroupCriterion--}
```
public GroupCriterion()
```


### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | الكائن للمقارنة مع هذا المثيل. |

**Returns:**
boolean - **True** إذا كان o هو GroupCriterion يحتوي على نفس قيمة UID لهذا الكائن؛ وإلا، **false**.
### getAscending() {#getAscending--}
```
public final boolean getAscending()
```


يحصل على قيمة تشير إلى ما إذا كان الحقل المستخدم كمعيار في تعريف المجموعة مُرتّبًا بترتيب تصاعدي. يكون False إذا كان الحقل مُرتّبًا بترتيب تنازلي.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان الحقل المستخدم كمعيار في تعريف المجموعة مُرتّبًا بترتيب تصاعدي.
### getCellColor() {#getCellColor--}
```
public final Color getCellColor()
```


يحصل على لون خلفية الخلية لحقل يُستخدم كمعيار في تعريف مجموعة.

**Returns:**
java.awt.Color - لون خلفية الخلية لحقل يُستخدم كمعيار في تعريف المجموعة.
### getField() {#getField--}
```
public final int getField()
```


يحصل على الحقل الذي يتم تجميعه.

**Returns:**
int - الحقل الذي يتم التجميع بناءً عليه.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


يحصل على الخط للمعيار في تعريف مجموعة.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font for a criterion in a group definition.
### getFontColor() {#getFontColor--}
```
public final Color getFontColor()
```


يحصل على لون الخط للحقل المستخدم كمعيار في تعريف مجموعة.

**Returns:**
java.awt.Color - لون الخط للحقل المستخدم كمعيار في تعريف المجموعة.
### getGroupInterval() {#getGroupInterval--}
```
public final Object getGroupInterval()
```


يحصل على الفاصل الزمني للحقل المستخدم كمعيار في تعريف مجموعة.

**Returns:**
java.lang.Object - الفاصل الزمني للحقل المستخدم كمعيار في تعريف المجموعة.
### getGroupOn() {#getGroupOn--}
```
public final int getGroupOn()
```


يحصل على نوع التجميع للحقل المستخدم كمعيار في تعريف مجموعة.

**Returns:**
int - نوع التجميع للحقل المستخدم كمعيار في تعريف المجموعة.
### getPattern() {#getPattern--}
```
public final int getPattern()
```


يحصل على نمط الخلية للحقل المستخدم كمعيار في تعريف مجموعة.

**Returns:**
int - نمط الخلية للحقل المستخدم كمعيار في تعريف المجموعة.
### getStartAt() {#getStartAt--}
```
public final Object getStartAt()
```


يحصل على بداية الفواصل الزمنية للحقل المستخدم كمعيار في تعريف مجموعة.

**Returns:**
java.lang.Object - بداية الفواصل للحقل المستخدم كمعيار في تعريف المجموعة.
### hashCode() {#hashCode--}
```
public int hashCode()
```


يعمل كدالة تجزئة لنوع معين.

**Returns:**
int - رمز تجزئة للكائن الحالي.
### setAscending(boolean value) {#setAscending-boolean-}
```
public final void setAscending(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان الحقل المستخدم كمعيار في تعريف المجموعة مُرتّبًا بترتيب تصاعدي. يكون False إذا كان الحقل مُرتّبًا بترتيب تنازلي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان الحقل المستخدم كمعيار في تعريف المجموعة مُرتّبًا بترتيب تصاعدي. |

### setCellColor(Color value) {#setCellColor-java.awt.Color-}
```
public final void setCellColor(Color value)
```


يضبط لون خلفية الخلية لحقل يُستخدم كمعيار في تعريف المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color | لون خلفية الخلية لحقل يُستخدم كمعيار في تعريف المجموعة. |

### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


يضبط الحقل الذي يتم التجميع بناءً عليه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | الحقل الذي يتم التجميع بناءً عليه. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


يضبط الخط للمعيار في تعريف المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | الخط للمعيار في تعريف المجموعة. |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public final void setFontColor(Color value)
```


يضبط لون الخط للحقل المستخدم كمعيار في تعريف المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color | لون الخط لحقل يُستخدم كمعيار في تعريف المجموعة. |

### setGroupInterval(Object value) {#setGroupInterval-java.lang.Object-}
```
public final void setGroupInterval(Object value)
```


يضبط الفاصل الزمني للحقل المستخدم كمعيار في تعريف المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object | الفاصل لحقل يُستخدم كمعيار في تعريف المجموعة. |

### setGroupOn(int value) {#setGroupOn-int-}
```
public final void setGroupOn(int value)
```


يضبط نوع التجميع للحقل المستخدم كمعيار في تعريف المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نوع التجميع لحقل يُستخدم كمعيار في تعريف المجموعة. |

### setPattern(int value) {#setPattern-int-}
```
public final void setPattern(int value)
```


يضبط نمط الخلية للحقل المستخدم كمعيار في تعريف المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نمط الخلية لحقل يُستخدم كمعيار في تعريف المجموعة. |

### setStartAt(Object value) {#setStartAt-java.lang.Object-}
```
public final void setStartAt(Object value)
```


يضبط بداية الفواصل للحقل المستخدم كمعيار في تعريف المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object | بداية الفواصل لحقل يُستخدم كمعيار في تعريف المجموعة. |

