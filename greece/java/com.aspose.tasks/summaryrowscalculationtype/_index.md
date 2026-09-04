---
title: "SummaryRowsCalculationType"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Καθορίζει τον τύπο υπολογισμού της τιμής των προσαρμοσμένων χαρακτηριστικών για τις γραμμές σύνοψης."
type: docs
weight: 282
url: /el/java/com.aspose.tasks/summaryrowscalculationtype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class SummaryRowsCalculationType extends System.Enum
```

Καθορίζει τον τύπο υπολογισμού της τιμής του προσαρμοσμένου χαρακτηριστικού για γραμμές σύνοψης.
## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
| [None](#None) | Σημαίνει ότι η τιμή του προσαρμοσμένου χαρακτηριστικού για τις γραμμές σύνοψης δεν υπολογίζεται. |
| [Rollup](#Rollup) | Σημαίνει ότι η τιμή του προσαρμοσμένου χαρακτηριστικού για τις γραμμές σύνοψης υπολογίζεται χρησιμοποιώντας τη συνάρτηση rollup που ορίζεται στο `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)). |
| [UseFormula](#UseFormula) | Σημαίνει ότι η τιμή του προσαρμοσμένου χαρακτηριστικού για τις γραμμές σύνοψης υπολογίζεται χρησιμοποιώντας τη φόρμουλα που ορίζεται στο `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)). |
### None {#None}
```
public static final int None
```


Σημαίνει ότι η τιμή του προσαρμοσμένου χαρακτηριστικού για τις γραμμές σύνοψης δεν υπολογίζεται.

### Rollup {#Rollup}
```
public static final int Rollup
```


Σημαίνει ότι η τιμή του προσαρμοσμένου χαρακτηριστικού για τις γραμμές σύνοψης υπολογίζεται χρησιμοποιώντας τη συνάρτηση rollup που ορίζεται στο `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)).

### UseFormula {#UseFormula}
```
public static final int UseFormula
```


Σημαίνει ότι η τιμή του προσαρμοσμένου χαρακτηριστικού για τις γραμμές σύνοψης υπολογίζεται χρησιμοποιώντας τη φόρμουλα που ορίζεται στο `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)).

--------------------

Για να λειτουργήσει αυτή η ρύθμιση, το `ExtendedAttributeDefinition.CalculationType`([ExtendedAttributeDefinition.getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [ExtendedAttributeDefinition.setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) πρέπει να οριστεί σε 'Formula'.

