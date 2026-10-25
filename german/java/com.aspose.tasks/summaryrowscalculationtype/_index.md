---
title: "SummaryRowsCalculationType"
second_title: "Aspose.Tasks for Java API Reference"
description: "Gibt den Typ der Berechnung des Werts benutzerdefinierter Attribute für Zusammenfassungszeilen an."
type: docs
weight: 282
url: /de/java/com.aspose.tasks/summaryrowscalculationtype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class SummaryRowsCalculationType extends System.Enum
```

Gibt den Typ einer Berechnung des Werts des benutzerdefinierten Attributs für Zusammenfassungszeilen an.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [None](#None) | Bedeutet, dass der Wert des benutzerdefinierten Attributs für Zusammenfassungszeilen nicht berechnet wird. |
| [Rollup](#Rollup) | Bedeutet, dass der Wert des benutzerdefinierten Attributs für Zusammenfassungszeilen mittels der Rollup-Funktion berechnet wird, die in `ExtendedAttributeDefinition.RollupType` definiert ist ([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)). |
| [UseFormula](#UseFormula) | Bedeutet, dass der Wert des benutzerdefinierten Attributs für Zusammenfassungszeilen mit der in `ExtendedAttributeDefinition.Formula` definierten Formel berechnet wird ([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)). |
### None {#None}
```
public static final int None
```


Bedeutet, dass der Wert des benutzerdefinierten Attributs für Zusammenfassungszeilen nicht berechnet wird.

### Rollup {#Rollup}
```
public static final int Rollup
```


Bedeutet, dass der Wert des benutzerdefinierten Attributs für Zusammenfassungszeilen mittels der Rollup-Funktion berechnet wird, die in `ExtendedAttributeDefinition.RollupType` definiert ist ([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)).

### UseFormula {#UseFormula}
```
public static final int UseFormula
```


Bedeutet, dass der Wert des benutzerdefinierten Attributs für Zusammenfassungszeilen mit der in `ExtendedAttributeDefinition.Formula` definierten Formel berechnet wird ([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)).

--------------------

Damit diese Einstellung funktioniert, muss `ExtendedAttributeDefinition.CalculationType`([ExtendedAttributeDefinition.getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [ExtendedAttributeDefinition.setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)) auf 'Formula' gesetzt werden.

