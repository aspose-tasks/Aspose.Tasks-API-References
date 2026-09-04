---
title: "SummaryRowsCalculationType"
second_title: "Aspose.Tasks for Java API 参考"
description: "指定汇总行自定义属性值的计算类型。"
type: docs
weight: 282
url: /zh/java/com.aspose.tasks/summaryrowscalculationtype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class SummaryRowsCalculationType extends System.Enum
```

指定自定义属性值在汇总行上的计算类型。
## 字段

| 字段 | 描述 |
| --- | --- |
| [None](#None) | 表示汇总行的自定义属性值未被计算。 |
| [Rollup](#Rollup) | 表示汇总行的自定义属性值是使用在 `ExtendedAttributeDefinition.RollupType` 中定义的汇总函数计算的([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)). |
| [UseFormula](#UseFormula) | 表示汇总行的自定义属性值是使用在 `ExtendedAttributeDefinition.Formula` 中定义的公式计算的([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)). |
### None {#None}
```
public static final int None
```


表示汇总行的自定义属性值未被计算。

### Rollup {#Rollup}
```
public static final int Rollup
```


表示汇总行的自定义属性值是使用在 `ExtendedAttributeDefinition.RollupType` 中定义的汇总函数计算的([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)).

### UseFormula {#UseFormula}
```
public static final int UseFormula
```


表示汇总行的自定义属性值是使用在 `ExtendedAttributeDefinition.Formula` 中定义的公式计算的([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)).

--------------------

要使此设置生效，`ExtendedAttributeDefinition.CalculationType`([ExtendedAttributeDefinition.getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [ExtendedAttributeDefinition.setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) 应设置为 'Formula'。

