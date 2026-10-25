---
title: "SummaryRowsCalculationType"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Spécifie le type de calcul de la valeur des attributs personnalisés pour les lignes de synthèse."
type: docs
weight: 282
url: /fr/java/com.aspose.tasks/summaryrowscalculationtype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class SummaryRowsCalculationType extends System.Enum
```

Spécifie le type de calcul de la valeur de l'attribut personnalisé pour les lignes de résumé.
## Champs

| Champ | Description |
| --- | --- |
| [None](#None) | Indique que la valeur de l'attribut personnalisé pour les lignes de synthèse n'est pas calculée. |
| [Rollup](#Rollup) | Indique que la valeur de l'attribut personnalisé pour les lignes de synthèse est calculée en utilisant la fonction d'agrégation définie dans `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)). |
| [UseFormula](#UseFormula) | Indique que la valeur de l'attribut personnalisé pour les lignes de synthèse est calculée en utilisant la formule définie dans `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)). |
### None {#None}
```
public static final int None
```


Indique que la valeur de l'attribut personnalisé pour les lignes de synthèse n'est pas calculée.

### Rollup {#Rollup}
```
public static final int Rollup
```


Indique que la valeur de l'attribut personnalisé pour les lignes de synthèse est calculée en utilisant la fonction d'agrégation définie dans `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)).

### UseFormula {#UseFormula}
```
public static final int UseFormula
```


Indique que la valeur de l'attribut personnalisé pour les lignes de synthèse est calculée en utilisant la formule définie dans `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)).

--------------------

Pour que ce paramètre fonctionne, `ExtendedAttributeDefinition.CalculationType`([ExtendedAttributeDefinition.getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [ExtendedAttributeDefinition.setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) doit être défini sur 'Formula'.

