---
title: "SummaryRowsCalculationType"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Especifica el tipo de cálculo del valor de los atributos personalizados para filas de resumen."
type: docs
weight: 282
url: /es/java/com.aspose.tasks/summaryrowscalculationtype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class SummaryRowsCalculationType extends System.Enum
```

Especifica el tipo de cálculo del valor del atributo personalizado para filas de resumen.
## Campos

| Campo | Descripción |
| --- | --- |
| [None](#None) | Indica que el valor del atributo personalizado para filas de resumen no se calcula. |
| [Rollup](#Rollup) | Indica que el valor del atributo personalizado para filas de resumen se calcula usando la función de acumulación definida en `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)). |
| [UseFormula](#UseFormula) | Indica que el valor del atributo personalizado para filas de resumen se calcula usando la fórmula definida en `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)). |
### None {#None}
```
public static final int None
```


Indica que el valor del atributo personalizado para filas de resumen no se calcula.

### Rollup {#Rollup}
```
public static final int Rollup
```


Indica que el valor del atributo personalizado para filas de resumen se calcula usando la función de acumulación definida en `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)).

### UseFormula {#UseFormula}
```
public static final int UseFormula
```


Indica que el valor del atributo personalizado para filas de resumen se calcula usando la fórmula definida en `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)).

--------------------

Para que esta configuración funcione, `ExtendedAttributeDefinition.CalculationType`([ExtendedAttributeDefinition.getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [ExtendedAttributeDefinition.setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) debe establecerse en 'Formula'.

