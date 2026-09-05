---
title: "SummaryRowsCalculationType"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Menentukan jenis perhitungan nilai atribut khusus untuk baris ringkasan."
type: docs
weight: 282
url: /id/java/com.aspose.tasks/summaryrowscalculationtype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class SummaryRowsCalculationType extends System.Enum
```

Menentukan jenis perhitungan nilai atribut khusus untuk baris ringkasan.
## Bidang

| Bidang | Deskripsi |
| --- | --- |
| [None](#None) | Berarti nilai atribut khusus untuk baris ringkasan tidak dihitung. |
| [Rollup](#Rollup) | Berarti nilai atribut khusus untuk baris ringkasan dihitung menggunakan fungsi rollup yang didefinisikan dalam `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)). |
| [UseFormula](#UseFormula) | Berarti nilai atribut khusus untuk baris ringkasan dihitung menggunakan formula yang didefinisikan dalam `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)). |
### None {#None}
```
public static final int None
```


Berarti nilai atribut khusus untuk baris ringkasan tidak dihitung.

### Rollup {#Rollup}
```
public static final int Rollup
```


Berarti nilai atribut khusus untuk baris ringkasan dihitung menggunakan fungsi rollup yang didefinisikan dalam `ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)).

### UseFormula {#UseFormula}
```
public static final int UseFormula
```


Berarti nilai atribut khusus untuk baris ringkasan dihitung menggunakan formula yang didefinisikan dalam `ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)).

--------------------

Agar pengaturan ini berfungsi, `ExtendedAttributeDefinition.CalculationType`([ExtendedAttributeDefinition.getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [ExtendedAttributeDefinition.setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) harus disetel ke 'Formula'.

