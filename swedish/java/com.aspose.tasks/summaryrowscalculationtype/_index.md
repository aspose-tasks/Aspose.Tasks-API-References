---
title: "SummaryRowsCalculationType"
second_title: "Aspose.Tasks for Java API-referens"
description: "Anger typen av beräkning av det anpassade attributets värde för sammanfattningsrader."
type: docs
weight: 282
url: /sv/java/com.aspose.tasks/summaryrowscalculationtype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class SummaryRowsCalculationType extends System.Enum
```

Anger typen av beräkning av det anpassade attributets värde för sammanfattningsrader.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [None](#None) | Betyder att det anpassade attributets värde för sammanfattningsrader inte beräknas. |
| [Rollup](#Rollup) | Betyder att det anpassade attributets värde för sammanfattningsrader beräknas med hjälp av sammanrullningsfunktion som definierats i `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)). |
| [UseFormula](#UseFormula) | Betyder att det anpassade attributets värde för sammanfattningsrader beräknas med hjälp av formel som definierats i `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)). |
### None {#None}
```
public static final int None
```


Betyder att det anpassade attributets värde för sammanfattningsrader inte beräknas.

### Rollup {#Rollup}
```
public static final int Rollup
```


Betyder att det anpassade attributets värde för sammanfattningsrader beräknas med hjälp av sammanrullningsfunktion som definierats i `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)).

### UseFormula {#UseFormula}
```
public static final int UseFormula
```


Betyder att det anpassade attributets värde för sammanfattningsrader beräknas med hjälp av formel som definierats i `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)).

--------------------

För att den här inställningen ska fungera bör `ExtendedAttributeDefinition.CalculationType`([ExtendedAttributeDefinition.getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [ExtendedAttributeDefinition.setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) sättas till 'Formula'.

