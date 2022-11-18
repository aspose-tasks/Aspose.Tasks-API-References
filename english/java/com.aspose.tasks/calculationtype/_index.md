---
title: CalculationType
second_title: Aspose.Tasks for Java API Reference
description: Specifies the type of a calculation of the custom attributes value.
type: docs
weight: 40
url: /java/com.aspose.tasks/calculationtype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class CalculationType extends System.Enum
```

Specifies the type of a calculation of the custom attribute's value.
## Fields

| Field | Description |
| --- | --- |
| [Formula](#Formula) | Means the value of the extended attribute is calculated using formula defined in  ExtendedAttributeDefinition.Formula ([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/[ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)). |
| [Lookup](#Lookup) | Means the value of the extended attribute is restricted to values from a lookup table. |
| [None](#None) | Means the extended attribute has no lookup table of formula and simply stores value set by the user. |
### Formula {#Formula}
```
public static final int Formula
```


Means the value of the extended attribute is calculated using formula defined in  ExtendedAttributeDefinition.Formula ([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/[ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)).

### Lookup {#Lookup}
```
public static final int Lookup
```


Means the value of the extended attribute is restricted to values from a lookup table.

### None {#None}
```
public static final int None
```


Means the extended attribute has no lookup table of formula and simply stores value set by the user.

