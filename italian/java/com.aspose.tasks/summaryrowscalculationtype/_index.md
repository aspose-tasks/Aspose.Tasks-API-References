---
title: "SummaryRowsCalculationType"
second_title: "Aspose.Tasks for Java API Reference"
description: "Specifica il tipo di calcolo del valore degli attributi personalizzati per le righe di riepilogo."
type: docs
weight: 282
url: /it/java/com.aspose.tasks/summaryrowscalculationtype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class SummaryRowsCalculationType extends System.Enum
```

Specifica il tipo di calcolo del valore dell'attributo personalizzato per le righe di riepilogo.
## Campi

| Campo | Descrizione |
| --- | --- |
| [None](#None) | Indica che il valore dell'attributo personalizzato per le righe di riepilogo non è calcolato. |
| [Rollup](#Rollup) | Indica che il valore dell'attributo personalizzato per le righe di riepilogo è calcolato utilizzando la funzione di aggregazione definita in `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)). |
| [UseFormula](#UseFormula) | Indica che il valore dell'attributo personalizzato per le righe di riepilogo è calcolato utilizzando la formula definita in `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)). |
### None {#None}
```
public static final int None
```


Indica che il valore dell'attributo personalizzato per le righe di riepilogo non è calcolato.

### Rollup {#Rollup}
```
public static final int Rollup
```


Indica che il valore dell'attributo personalizzato per le righe di riepilogo è calcolato utilizzando la funzione di aggregazione definita in `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)).

### UseFormula {#UseFormula}
```
public static final int UseFormula
```


Indica che il valore dell'attributo personalizzato per le righe di riepilogo è calcolato utilizzando la formula definita in `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)).

--------------------

Affinché questa impostazione funzioni, `ExtendedAttributeDefinition.CalculationType`([ExtendedAttributeDefinition.getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [ExtendedAttributeDefinition.setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) dovrebbe essere impostato su 'Formula'.

