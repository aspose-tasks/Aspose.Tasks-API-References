---
title: "SummaryRowsCalculationType"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Specificeert het type berekening van de waarde van aangepaste attributen voor samenvattingsrijen."
type: docs
weight: 282
url: /nl/java/com.aspose.tasks/summaryrowscalculationtype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class SummaryRowsCalculationType extends System.Enum
```

Specificeert het type van een berekening van de waarde van het aangepaste attribuut voor samenvattingsrijen.
## Velden

| Veld | Beschrijving |
| --- | --- |
| [None](#None) | Betekent dat de waarde van het aangepaste attribuut voor samenvattingsrijen niet wordt berekend. |
| [Rollup](#Rollup) | Betekent dat de waarde van het aangepaste attribuut voor samenvattingsrijen wordt berekend met behulp van de rollup-functie die is gedefinieerd in `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)). |
| [UseFormula](#UseFormula) | Betekent dat de waarde van het aangepaste attribuut voor samenvattingsrijen wordt berekend met behulp van de formule die is gedefinieerd in `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)). |
### None {#None}
```
public static final int None
```


Betekent dat de waarde van het aangepaste attribuut voor samenvattingsrijen niet wordt berekend.

### Rollup {#Rollup}
```
public static final int Rollup
```


Betekent dat de waarde van het aangepaste attribuut voor samenvattingsrijen wordt berekend met behulp van de rollup-functie die is gedefinieerd in `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)).

### UseFormula {#UseFormula}
```
public static final int UseFormula
```


Betekent dat de waarde van het aangepaste attribuut voor samenvattingsrijen wordt berekend met behulp van de formule die is gedefinieerd in `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)).

--------------------

Om deze instelling te laten werken, moet `ExtendedAttributeDefinition.CalculationType`([ExtendedAttributeDefinition.getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [ExtendedAttributeDefinition.setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) worden ingesteld op 'Formula'.

