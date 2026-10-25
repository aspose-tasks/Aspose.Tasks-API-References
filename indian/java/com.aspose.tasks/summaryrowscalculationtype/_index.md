---
title: "SummaryRowsCalculationType"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "सारांश पंक्तियों के लिए कस्टम एट्रिब्यूट्स मान की गणना के प्रकार को निर्दिष्ट करता है।"
type: docs
weight: 282
url: /hi/java/com.aspose.tasks/summaryrowscalculationtype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class SummaryRowsCalculationType extends System.Enum
```

सारांश पंक्तियों के लिए कस्टम एट्रिब्यूट मान की गणना के प्रकार को निर्दिष्ट करता है।
## फ़ील्ड्स

| फ़ील्ड | विवरण |
| --- | --- |
| [None](#None) | अर्थात कस्टम एट्रिब्यूट का मान सारांश पंक्तियों के लिए गणना नहीं किया जाता। |
| [Rollup](#Rollup) | अर्थात कस्टम एट्रिब्यूट का मान सारांश पंक्तियों के लिए `ExtendedAttributeDefinition.RollupType` में परिभाषित रोलअप फ़ंक्शन का उपयोग करके गणना किया जाता है ([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)). |
| [UseFormula](#UseFormula) | अर्थात कस्टम एट्रिब्यूट का मान सारांश पंक्तियों के लिए `ExtendedAttributeDefinition.Formula` में परिभाषित फ़ॉर्मूला का उपयोग करके गणना किया जाता है ([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)). |
### None {#None}
```
public static final int None
```


अर्थात कस्टम एट्रिब्यूट का मान सारांश पंक्तियों के लिए गणना नहीं किया जाता।

### Rollup {#Rollup}
```
public static final int Rollup
```


अर्थात कस्टम एट्रिब्यूट का मान सारांश पंक्तियों के लिए `ExtendedAttributeDefinition.RollupType` में परिभाषित रोलअप फ़ंक्शन का उपयोग करके गणना किया जाता है ([ExtendedAttributeDefinition.getRollupType()](../../com.aspose.tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose.tasks/extendedattributedefinition\#setRollupType-int-)).

### UseFormula {#UseFormula}
```
public static final int UseFormula
```


अर्थात कस्टम एट्रिब्यूट का मान सारांश पंक्तियों के लिए `ExtendedAttributeDefinition.Formula` में परिभाषित फ़ॉर्मूला का उपयोग करके गणना किया जाता है ([ExtendedAttributeDefinition.getFormula()](../../com.aspose.tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose.tasks/extendedattributedefinition\#setFormula-String-)).

--------------------

इस सेटिंग के काम करने के लिए, `ExtendedAttributeDefinition.CalculationType` ([ExtendedAttributeDefinition.getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [ExtendedAttributeDefinition.setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) को 'Formula' पर सेट किया जाना चाहिए।

