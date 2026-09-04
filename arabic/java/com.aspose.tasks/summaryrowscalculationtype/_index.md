---
title: "SummaryRowsCalculationType"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يحدد نوع حساب قيمة السمات المخصصة للصفوف الملخصة."
type: docs
weight: 282
url: /ar/java/com.aspose.tasks/summaryrowscalculationtype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class SummaryRowsCalculationType extends System.Enum
```

يحدد نوع حساب قيمة السمة المخصصة لصفوف الملخص.
## الحقول

| حقل | الوصف |
| --- | --- |
| [None](#None) | يعني أن قيمة السمة المخصصة للصفوف الملخصة غير محسوبة. |
| [Rollup](#Rollup) | يعني أن قيمة السمة المخصصة للصفوف الملخصة تُحسب باستخدام دالة التجميع المعرفة في `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)). |
| [UseFormula](#UseFormula) | يعني أن قيمة السمة المخصصة للصفوف الملخصة تُحسب باستخدام الصيغة المعرفة في `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)). |
### None {#None}
```
public static final int None
```


يعني أن قيمة السمة المخصصة للصفوف الملخصة غير محسوبة.

### Rollup {#Rollup}
```
public static final int Rollup
```


يعني أن قيمة السمة المخصصة للصفوف الملخصة تُحسب باستخدام دالة التجميع المعرفة في `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)).

### UseFormula {#UseFormula}
```
public static final int UseFormula
```


يعني أن قيمة السمة المخصصة للصفوف الملخصة تُحسب باستخدام الصيغة المعرفة في `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)).

--------------------

لكي يعمل هذا الإعداد، يجب تعيين `ExtendedAttributeDefinition.CalculationType`([ExtendedAttributeDefinition.getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [ExtendedAttributeDefinition.setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) إلى 'Formula'.

