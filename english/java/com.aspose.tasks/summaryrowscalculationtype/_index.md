---
title: SummaryRowsCalculationType
second_title: Aspose.Tasks for Java API Reference
description: Specifies the type of a calculation of the custom attributes value for summary rows.
type: docs
weight: 281
url: /java/com.aspose.tasks/summaryrowscalculationtype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class SummaryRowsCalculationType extends System.Enum
```

Specifies the type of a calculation of the custom attribute's value for summary rows.
## Fields

| Field | Description |
| --- | --- |
| [None](#None) | Means the custom attribute's value for summary rows is not calculated. |
| [Rollup](#Rollup) | Means the custom attribute's value for summary rows is calculated using rollup function defined in `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)). |
| [UseFormula](#UseFormula) | Means the custom attribute's value for summary rows is calculated using formula defined in `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula\_Rename\_Namesake()](../../com.aspose.tasks/extendedattributedefinition\#getFormula-Rename-Namesake--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)). |
### None {#None}
```
public static final int None
```


Means the custom attribute's value for summary rows is not calculated.

### Rollup {#Rollup}
```
public static final int Rollup
```


Means the custom attribute's value for summary rows is calculated using rollup function defined in `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)).

### UseFormula {#UseFormula}
```
public static final int UseFormula
```


Means the custom attribute's value for summary rows is calculated using formula defined in `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula\_Rename\_Namesake()](../../com.aspose.tasks/extendedattributedefinition\#getFormula-Rename-Namesake--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)).

--------------------

For this setting to work, `ExtendedAttributeDefinition.CalculationType`([ExtendedAttributeDefinition.getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [ExtendedAttributeDefinition.setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) should be set to 'Formula'.

