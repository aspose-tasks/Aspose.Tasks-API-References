---
title: "PrimaveraTaskProperties"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل خصائص خاصة بـ Primavera لمهمة تُقرأ من ملفات Primavera XER أو P6XML."
type: docs
weight: 209
url: /ar/java/com.aspose.tasks/primaverataskproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraTaskProperties
```

يمثل خصائص خاصة بـ Primavera لمهمة تُقرأ من ملفات Primavera (XER أو P6XML).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getActivityId()](#getActivityId--) | يحصل على حقل معرف النشاط - المعرف الفريد للمهمة المستخدم في Primavera. |
| [getActivityType()](#getActivityType--) | يحصل على قيمة الحقل 'Activity Type'. |
| [getActualExpenseCost()](#getActualExpenseCost--) | يحصل على قيمة تكلفة المصروف الفعلية. |
| [getActualLaborCost()](#getActualLaborCost--) | يحصل على قيمة تكلفة العمالة الفعلية . |
| [getActualLaborUnits()](#getActualLaborUnits--) | يحصل على قيمة وحدات العمالة الفعلية. |
| [getActualMaterialCost()](#getActualMaterialCost--) | يحصل على قيمة تكلفة المواد الفعلية. |
| [getActualNonLaborUnits()](#getActualNonLaborUnits--) | يحصل على قيمة وحدات غير العمالة الفعلية. |
| [getActualNonlaborCost()](#getActualNonlaborCost--) | يحصل على قيمة تكلفة غير العمالة الفعلية . |
| [getActualTotalCost()](#getActualTotalCost--) | يحصل على القيمة الإجمالية للتكاليف الفعلية. |
| [getBudgetedExpenseCost()](#getBudgetedExpenseCost--) | يحصل على قيمة تكلفة النفقات المتوقعة (أو المخططة). |
| [getBudgetedLaborCost()](#getBudgetedLaborCost--) | يحصل على قيمة تكلفة العمالة المتوقعة (أو المخططة) . |
| [getBudgetedMaterialCost()](#getBudgetedMaterialCost--) | يحصل على قيمة تكلفة المواد المتوقعة (أو المخططة). |
| [getBudgetedNonlaborCost()](#getBudgetedNonlaborCost--) | يحصل على قيمة تكلفة غير العمالة المتوقعة (أو المخططة) . |
| [getBudgetedTotalCost()](#getBudgetedTotalCost--) | يحصل على القيمة الإجمالية للتكاليف المتوقعة (أو المخططة). |
| [getDurationPercentComplete()](#getDurationPercentComplete--) | يحصل على قيمة نسبة إكمال المدة. |
| [getDurationType()](#getDurationType--) | يحصل على قيمة حقل 'نوع المدة' للنشاط. |
| [getPercentCompleteType()](#getPercentCompleteType--) | يحصل على قيمة حقل '% نوع الإكمال' للنشاط. |
| [getPhysicalPercentComplete()](#getPhysicalPercentComplete--) | يحصل على قيمة النسبة المئوية الفعلية. |
| [getPlannedDuration()](#getPlannedDuration--) | يحصل على المدة الأصلية أو المخططة -- إجمالي وقت العمل من تاريخ بدء المهمة المخطط إلى تاريخ الانتهاء المخطط.. |
| [getPrimaryConstraintDate()](#getPrimaryConstraintDate--) | يحصل على تاريخ القيد الأساسي. |
| [getPrimaryConstraintType()](#getPrimaryConstraintType--) | يحصل على نوع القيد الأساسي. |
| [getRawActivityType()](#getRawActivityType--) | يحصل على تمثيل النص الخام (كما في ملف المصدر) لحقل 'نوع النشاط' للنشاط. |
| [getRawCompletePercentType()](#getRawCompletePercentType--) | يحصل على تمثيل النص الخام (كما في ملف المصدر) لحقل '% نوع الإكمال' للنشاط. |
| [getRawDurationType()](#getRawDurationType--) | يحصل على تمثيل النص الخام (كما في ملف المصدر) لحقل 'نوع المدة' للنشاط. |
| [getRawStatus()](#getRawStatus--) | يحصل على تمثيل النص الخام (كما في ملف المصدر) لحقل 'الحالة' للنشاط. |
| [getRemainingEarlyFinish()](#getRemainingEarlyFinish--) | يحصل على تاريخ الانتهاء المبكر المتبقي - التاريخ الذي من المقرر أن يكتمل فيه العمل المتبقي للنشاط. |
| [getRemainingEarlyStart()](#getRemainingEarlyStart--) | يحصل على تاريخ البدء المبكر المتبقي - التاريخ الذي من المقرر أن يبدأ فيه العمل المتبقي للنشاط. |
| [getRemainingExpenseCost()](#getRemainingExpenseCost--) | يحصل على قيمة تكلفة النفقات المتبقية. |
| [getRemainingLaborUnits()](#getRemainingLaborUnits--) | يحصل على قيمة وحدات العمل المتبقية. |
| [getRemainingLateFinish()](#getRemainingLateFinish--) | يحصل على تاريخ الانتهاء المتأخر المتبقي. |
| [getRemainingLateStart()](#getRemainingLateStart--) | يحصل على تاريخ البدء المتأخر المتبقي. |
| [getRemainingNonLaborUnits()](#getRemainingNonLaborUnits--) | يحصل على قيمة وحدات غير العمل المتبقية. |
| [getSecondaryConstraintDate()](#getSecondaryConstraintDate--) | يحصل على تاريخ القيد الثانوي. |
| [getSecondaryConstraintType()](#getSecondaryConstraintType--) | يحصل على نوع القيد الثانوي. |
| [getSequenceNumber()](#getSequenceNumber--) | يحصل على رقم التسلسل لعنصر WBS (المهام الملخصة). |
| [getUnitsPercentComplete()](#getUnitsPercentComplete--) | يحصل على قيمة نسبة إكمال الوحدات. |
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


يحصل على حقل معرف النشاط - المعرف الفريد للمهمة المستخدم في Primavera.

--------------------

ينطبق فقط على الأنشطة (المهام غير الملخصة).

**Returns:**
java.lang.String - حقل معرف النشاط - معرف فريد للمهمة يستخدم في Primavera.
### getActivityType() {#getActivityType--}
```
public final int getActivityType()
```


يحصل على قيمة الحقل 'Activity Type'.

--------------------

ينطبق فقط على الأنشطة (المهام غير الملخصة).

**Returns:**
int - قيمة حقل 'Activity Type'.
### getActualExpenseCost() {#getActualExpenseCost--}
```
public final BigDecimal getActualExpenseCost()
```


يحصل على قيمة تكلفة المصروف الفعلية.

**Returns:**
java.math.BigDecimal - قيمة تكلفة المصروف الفعلية.
### getActualLaborCost() {#getActualLaborCost--}
```
public final BigDecimal getActualLaborCost()
```


يحصل على قيمة تكلفة العمالة الفعلية .

**Returns:**
java.math.BigDecimal - قيمة تكلفة العمل الفعلية .
### getActualLaborUnits() {#getActualLaborUnits--}
```
public final double getActualLaborUnits()
```


يحصل على قيمة وحدات العمالة الفعلية.

**Returns:**
double - قيمة وحدات العمل الفعلية.
### getActualMaterialCost() {#getActualMaterialCost--}
```
public final BigDecimal getActualMaterialCost()
```


يحصل على قيمة تكلفة المواد الفعلية.

**Returns:**
java.math.BigDecimal - قيمة تكلفة المادة الفعلية.
### getActualNonLaborUnits() {#getActualNonLaborUnits--}
```
public final double getActualNonLaborUnits()
```


يحصل على قيمة وحدات غير العمالة الفعلية.

**Returns:**
double - قيمة وحدات غير العمل الفعلية.
### getActualNonlaborCost() {#getActualNonlaborCost--}
```
public final BigDecimal getActualNonlaborCost()
```


يحصل على قيمة تكلفة غير العمالة الفعلية .

**Returns:**
java.math.BigDecimal - قيمة تكلفة غير العمل الفعلية .
### getActualTotalCost() {#getActualTotalCost--}
```
public final BigDecimal getActualTotalCost()
```


يحصل على القيمة الإجمالية للتكاليف الفعلية.

**Returns:**
java.math.BigDecimal - القيمة الإجمالية للتكاليف الفعلية.
### getBudgetedExpenseCost() {#getBudgetedExpenseCost--}
```
public final BigDecimal getBudgetedExpenseCost()
```


يحصل على قيمة تكلفة النفقات المتوقعة (أو المخططة).

**Returns:**
java.math.BigDecimal - قيمة تكلفة المصروف المتوقعة (أو المخططة).
### getBudgetedLaborCost() {#getBudgetedLaborCost--}
```
public final BigDecimal getBudgetedLaborCost()
```


يحصل على قيمة تكلفة العمالة المتوقعة (أو المخططة) .

**Returns:**
java.math.BigDecimal - قيمة تكلفة العمل المتوقعة (أو المخططة) .
### getBudgetedMaterialCost() {#getBudgetedMaterialCost--}
```
public final BigDecimal getBudgetedMaterialCost()
```


يحصل على قيمة تكلفة المواد المتوقعة (أو المخططة).

**Returns:**
java.math.BigDecimal - قيمة تكلفة المادة المتوقعة (أو المخططة).
### getBudgetedNonlaborCost() {#getBudgetedNonlaborCost--}
```
public final BigDecimal getBudgetedNonlaborCost()
```


يحصل على قيمة تكلفة غير العمالة المتوقعة (أو المخططة) .

**Returns:**
java.math.BigDecimal - قيمة تكلفة غير العمل المتوقعة (أو المخططة) .
### getBudgetedTotalCost() {#getBudgetedTotalCost--}
```
public final BigDecimal getBudgetedTotalCost()
```


يحصل على القيمة الإجمالية للتكاليف المتوقعة (أو المخططة).

**Returns:**
java.math.BigDecimal - القيمة الإجمالية للتكاليف المتوقعة (أو المخططة).
### getDurationPercentComplete() {#getDurationPercentComplete--}
```
public final double getDurationPercentComplete()
```


يحصل على قيمة نسبة إكمال المدة.

**Returns:**
double - قيمة نسبة إكمال المدة.
### getDurationType() {#getDurationType--}
```
public final int getDurationType()
```


يحصل على قيمة حقل 'نوع المدة' للنشاط.

--------------------

ينطبق فقط على الأنشطة (المهام غير الملخصة).

**Returns:**
int - قيمة حقل 'Duration Type' للنشاط.
### getPercentCompleteType() {#getPercentCompleteType--}
```
public final int getPercentCompleteType()
```


يحصل على قيمة حقل '% نوع الإكمال' للنشاط.

--------------------

ينطبق فقط على الأنشطة (المهام غير الملخصة).

**Returns:**
int - قيمة حقل '% Complete Type' للنشاط.
### getPhysicalPercentComplete() {#getPhysicalPercentComplete--}
```
public final double getPhysicalPercentComplete()
```


يحصل على قيمة النسبة المئوية الفعلية.

--------------------

ينطبق فقط على الأنشطة (المهام غير الملخصة).

**Returns:**
double - قيمة Physical Percent Complete.
### getPlannedDuration() {#getPlannedDuration--}
```
public final Duration getPlannedDuration()
```


يحصل على المدة الأصلية أو المخططة -- إجمالي وقت العمل من تاريخ بدء المهمة المخطط إلى تاريخ الانتهاء المخطط..

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the original or planned duration -- the total working time from the task planned start date to the planned finish date.
### getPrimaryConstraintDate() {#getPrimaryConstraintDate--}
```
public final Date getPrimaryConstraintDate()
```


يحصل على تاريخ القيد الأساسي.

**Returns:**
java.util.Date - تاريخ القيد الأساسي.
### getPrimaryConstraintType() {#getPrimaryConstraintType--}
```
public final int getPrimaryConstraintType()
```


يحصل على نوع القيد الأساسي.

**Returns:**
int - نوع القيد الأساسي.
### getRawActivityType() {#getRawActivityType--}
```
public final String getRawActivityType()
```


يحصل على تمثيل النص الخام (كما في ملف المصدر) لحقل 'نوع النشاط' للنشاط.

--------------------

ينطبق فقط على الأنشطة (المهام غير الملخصة).

**Returns:**
java.lang.String - تمثيل النص الخام (كما في ملف المصدر) لحقل 'Activity Type' للنشاط.
### getRawCompletePercentType() {#getRawCompletePercentType--}
```
public final String getRawCompletePercentType()
```


يحصل على تمثيل النص الخام (كما في ملف المصدر) لحقل '% نوع الإكمال' للنشاط.

--------------------

ينطبق فقط على الأنشطة (المهام غير الملخصة).

**Returns:**
java.lang.String - تمثيل النص الخام (كما في ملف المصدر) لحقل '% Complete Type' للنشاط.
### getRawDurationType() {#getRawDurationType--}
```
public final String getRawDurationType()
```


يحصل على تمثيل النص الخام (كما في ملف المصدر) لحقل 'نوع المدة' للنشاط.

--------------------

ينطبق فقط على الأنشطة (المهام غير الملخصة).

**Returns:**
java.lang.String - تمثيل النص الخام (كما في ملف المصدر) لحقل 'Duration Type' للنشاط.
### getRawStatus() {#getRawStatus--}
```
public final String getRawStatus()
```


يحصل على تمثيل النص الخام (كما في ملف المصدر) لحقل 'الحالة' للنشاط.

--------------------

ينطبق فقط على الأنشطة (المهام غير الملخصة).

**Returns:**
java.lang.String - تمثيل النص الخام (كما في ملف المصدر) لحقل 'Status' للنشاط.
### getRemainingEarlyFinish() {#getRemainingEarlyFinish--}
```
public final Date getRemainingEarlyFinish()
```


يحصل على تاريخ الانتهاء المبكر المتبقي - التاريخ الذي من المقرر أن يكتمل فيه العمل المتبقي للنشاط.

**Returns:**
java.util.Date - تاريخ الانتهاء المبكر المتبقي - التاريخ الذي من المقرر فيه إكمال العمل المتبقي للنشاط.
### getRemainingEarlyStart() {#getRemainingEarlyStart--}
```
public final Date getRemainingEarlyStart()
```


يحصل على تاريخ البدء المبكر المتبقي - التاريخ الذي من المقرر أن يبدأ فيه العمل المتبقي للنشاط.

**Returns:**
java.util.Date - تاريخ البدء المبكر المتبقي - التاريخ الذي من المقرر فيه بدء العمل المتبقي للنشاط.
### getRemainingExpenseCost() {#getRemainingExpenseCost--}
```
public final BigDecimal getRemainingExpenseCost()
```


يحصل على قيمة تكلفة النفقات المتبقية.

**Returns:**
java.math.BigDecimal - قيمة تكلفة النفقات المتبقية.
### getRemainingLaborUnits() {#getRemainingLaborUnits--}
```
public final double getRemainingLaborUnits()
```


يحصل على قيمة وحدات العمل المتبقية.

**Returns:**
double - قيمة وحدات العمل المتبقية.
### getRemainingLateFinish() {#getRemainingLateFinish--}
```
public final Date getRemainingLateFinish()
```


يحصل على تاريخ الانتهاء المتأخر المتبقي.

**Returns:**
java.util.Date - تاريخ الانتهاء المتأخر المتبقي.
### getRemainingLateStart() {#getRemainingLateStart--}
```
public final Date getRemainingLateStart()
```


يحصل على تاريخ البدء المتأخر المتبقي.

**Returns:**
java.util.Date - تاريخ البدء المتأخر المتبقي.
### getRemainingNonLaborUnits() {#getRemainingNonLaborUnits--}
```
public final double getRemainingNonLaborUnits()
```


يحصل على قيمة وحدات غير العمل المتبقية.

**Returns:**
double - قيمة وحدات غير العمل المتبقية.
### getSecondaryConstraintDate() {#getSecondaryConstraintDate--}
```
public final Date getSecondaryConstraintDate()
```


يحصل على تاريخ القيد الثانوي.

**Returns:**
java.util.Date - تاريخ القيد الثانوي.
### getSecondaryConstraintType() {#getSecondaryConstraintType--}
```
public final int getSecondaryConstraintType()
```


يحصل على نوع القيد الثانوي.

**Returns:**
int - نوع القيد الثانوي.
### getSequenceNumber() {#getSequenceNumber--}
```
public final int getSequenceNumber()
```


يحصل على رقم التسلسل لعنصر WBS (المهام الملخصة). يُستخدم لترتيب المهام الملخصة في Primavera.

--------------------

قابل للتطبيق على عناصر WBS (المهام الملخصة).

**Returns:**
int - رقم التسلسل لعنصر WBS (المهام الملخصة).
### getUnitsPercentComplete() {#getUnitsPercentComplete--}
```
public final double getUnitsPercentComplete()
```


يحصل على قيمة نسبة إكمال الوحدات.

**Returns:**
double - قيمة نسبة إكمال الوحدات.
