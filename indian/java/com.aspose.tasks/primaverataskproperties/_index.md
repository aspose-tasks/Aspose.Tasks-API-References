---
title: "PrimaveraTaskProperties"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "Primavera-विशिष्ट गुणों को दर्शाता है जो एक कार्य के लिए Primavera फ़ाइलों XER या P6XML से पढ़े जाते हैं।"
type: docs
weight: 209
url: /hi/java/com.aspose.tasks/primaverataskproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraTaskProperties
```

Primavera फ़ाइलों (XER या P6XML) से पढ़े गए टास्क के लिए Primavera-विशिष्ट गुण दर्शाता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getActivityId()](#getActivityId--) | एक activity id फ़ील्ड प्राप्त करता है - वह कार्य का अद्वितीय पहचानकर्ता जो Primavera द्वारा उपयोग किया जाता है। |
| [getActivityType()](#getActivityType--) | 'Activity Type' फ़ील्ड का मान प्राप्त करता है। |
| [getActualExpenseCost()](#getActualExpenseCost--) | वास्तविक खर्च लागत का मान प्राप्त करता है। |
| [getActualLaborCost()](#getActualLaborCost--) | वास्तविक श्रम लागत का मान प्राप्त करता है . |
| [getActualLaborUnits()](#getActualLaborUnits--) | वास्तविक श्रम इकाइयों का मान प्राप्त करता है। |
| [getActualMaterialCost()](#getActualMaterialCost--) | वास्तविक सामग्री लागत का मान प्राप्त करता है। |
| [getActualNonLaborUnits()](#getActualNonLaborUnits--) | वास्तविक गैर-श्रम इकाइयों का मान प्राप्त करता है। |
| [getActualNonlaborCost()](#getActualNonlaborCost--) | वास्तविक गैर-श्रम लागत का मान प्राप्त करता है . |
| [getActualTotalCost()](#getActualTotalCost--) | वास्तविक लागतों का कुल मान प्राप्त करता है। |
| [getBudgetedExpenseCost()](#getBudgetedExpenseCost--) | बजटेड (या नियोजित) खर्च लागत का मान प्राप्त करता है। |
| [getBudgetedLaborCost()](#getBudgetedLaborCost--) | बजटेड (या नियोजित) श्रम लागत का मान प्राप्त करता है . |
| [getBudgetedMaterialCost()](#getBudgetedMaterialCost--) | बजटेड (या नियोजित) सामग्री लागत का मान प्राप्त करता है। |
| [getBudgetedNonlaborCost()](#getBudgetedNonlaborCost--) | बजटेड (या नियोजित) गैर-श्रम लागत का मान प्राप्त करता है . |
| [getBudgetedTotalCost()](#getBudgetedTotalCost--) | बजटेड (या नियोजित) लागतों का कुल मान प्राप्त करता है। |
| [getDurationPercentComplete()](#getDurationPercentComplete--) | अवधि प्रतिशत पूर्णता का मान प्राप्त करता है। |
| [getDurationType()](#getDurationType--) | गतिविधि के 'Duration Type' फ़ील्ड का मान प्राप्त करता है। |
| [getPercentCompleteType()](#getPercentCompleteType--) | गतिविधि के '% Complete Type' फ़ील्ड का मान प्राप्त करता है। |
| [getPhysicalPercentComplete()](#getPhysicalPercentComplete--) | भौतिक प्रतिशत पूर्णता का मान प्राप्त करता है। |
| [getPlannedDuration()](#getPlannedDuration--) | मूल या नियोजित अवधि प्राप्त करता है -- कार्य की नियोजित प्रारंभ तिथि से नियोजित समाप्ति तिथि तक का कुल कार्य समय.. |
| [getPrimaryConstraintDate()](#getPrimaryConstraintDate--) | प्राथमिक प्रतिबंध की तिथि प्राप्त करता है। |
| [getPrimaryConstraintType()](#getPrimaryConstraintType--) | प्राथमिक प्रतिबंध का प्रकार प्राप्त करता है। |
| [getRawActivityType()](#getRawActivityType--) | गतिविधि के 'Activity Type' फ़ील्ड का कच्चा पाठ प्रतिनिधित्व (जैसे स्रोत फ़ाइल में) प्राप्त करता है। |
| [getRawCompletePercentType()](#getRawCompletePercentType--) | गतिविधि के '% Complete Type' फ़ील्ड का कच्चा पाठ प्रतिनिधित्व (जैसे स्रोत फ़ाइल में) प्राप्त करता है। |
| [getRawDurationType()](#getRawDurationType--) | गतिविधि के 'Duration Type' फ़ील्ड का कच्चा पाठ प्रतिनिधित्व (जैसे स्रोत फ़ाइल में) प्राप्त करता है। |
| [getRawStatus()](#getRawStatus--) | गतिविधि के 'Status' फ़ील्ड का कच्चा पाठ प्रतिनिधित्व (जैसे स्रोत फ़ाइल में) प्राप्त करता है। |
| [getRemainingEarlyFinish()](#getRemainingEarlyFinish--) | शेष प्रारंभिक समाप्ति तिथि प्राप्त करता है - वह तिथि जब गतिविधि के शेष कार्य को समाप्त करने के लिए निर्धारित किया गया है। |
| [getRemainingEarlyStart()](#getRemainingEarlyStart--) | शेष प्रारंभिक प्रारंभ तिथि प्राप्त करता है - वह तिथि जब गतिविधि के शेष कार्य को शुरू करने के लिए निर्धारित किया गया है। |
| [getRemainingExpenseCost()](#getRemainingExpenseCost--) | शेष खर्च लागत का मान प्राप्त करता है। |
| [getRemainingLaborUnits()](#getRemainingLaborUnits--) | शेष श्रम इकाइयों का मान प्राप्त करता है। |
| [getRemainingLateFinish()](#getRemainingLateFinish--) | शेष देर से समाप्ति तिथि प्राप्त करता है। |
| [getRemainingLateStart()](#getRemainingLateStart--) | शेष देर से प्रारंभ तिथि प्राप्त करता है। |
| [getRemainingNonLaborUnits()](#getRemainingNonLaborUnits--) | शेष गैर-श्रम इकाइयों का मान प्राप्त करता है। |
| [getSecondaryConstraintDate()](#getSecondaryConstraintDate--) | द्वितीयक प्रतिबंध की तिथि प्राप्त करता है। |
| [getSecondaryConstraintType()](#getSecondaryConstraintType--) | द्वितीयक प्रतिबंध का प्रकार प्राप्त करता है। |
| [getSequenceNumber()](#getSequenceNumber--) | WBS आइटम (सारांश कार्य) का क्रमांक प्राप्त करता है। |
| [getUnitsPercentComplete()](#getUnitsPercentComplete--) | इकाइयों के प्रतिशत पूर्णता का मान प्राप्त करता है। |
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


एक activity id फ़ील्ड प्राप्त करता है - वह कार्य का अद्वितीय पहचानकर्ता जो Primavera द्वारा उपयोग किया जाता है।

--------------------

केवल गतिविधियों (गैर-सारांश कार्य) के लिए लागू है।

**Returns:**
java.lang.String - एक गतिविधि आईडी फ़ील्ड - प्रिमावेरा द्वारा उपयोग किया जाने वाला कार्य का अद्वितीय पहचानकर्ता।
### getActivityType() {#getActivityType--}
```
public final int getActivityType()
```


'Activity Type' फ़ील्ड का मान प्राप्त करता है।

--------------------

केवल गतिविधियों (गैर-सारांश कार्य) के लिए लागू है।

**Returns:**
int - 'Activity Type' फ़ील्ड का मान।
### getActualExpenseCost() {#getActualExpenseCost--}
```
public final BigDecimal getActualExpenseCost()
```


वास्तविक खर्च लागत का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - वास्तविक खर्च लागत का मान।
### getActualLaborCost() {#getActualLaborCost--}
```
public final BigDecimal getActualLaborCost()
```


वास्तविक श्रम लागत का मान प्राप्त करता है .

**Returns:**
java.math.BigDecimal - वास्तविक श्रम लागत का मान।
### getActualLaborUnits() {#getActualLaborUnits--}
```
public final double getActualLaborUnits()
```


वास्तविक श्रम इकाइयों का मान प्राप्त करता है।

**Returns:**
double - वास्तविक श्रम इकाइयों का मान।
### getActualMaterialCost() {#getActualMaterialCost--}
```
public final BigDecimal getActualMaterialCost()
```


वास्तविक सामग्री लागत का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - वास्तविक सामग्री लागत का मान।
### getActualNonLaborUnits() {#getActualNonLaborUnits--}
```
public final double getActualNonLaborUnits()
```


वास्तविक गैर-श्रम इकाइयों का मान प्राप्त करता है।

**Returns:**
double - वास्तविक गैर-श्रम इकाइयों का मान।
### getActualNonlaborCost() {#getActualNonlaborCost--}
```
public final BigDecimal getActualNonlaborCost()
```


वास्तविक गैर-श्रम लागत का मान प्राप्त करता है .

**Returns:**
java.math.BigDecimal - वास्तविक गैर-श्रम लागत का मान।
### getActualTotalCost() {#getActualTotalCost--}
```
public final BigDecimal getActualTotalCost()
```


वास्तविक लागतों का कुल मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - वास्तविक लागतों का कुल मान।
### getBudgetedExpenseCost() {#getBudgetedExpenseCost--}
```
public final BigDecimal getBudgetedExpenseCost()
```


बजटेड (या नियोजित) खर्च लागत का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - बजटेड (या नियोजित) खर्च लागत का मान।
### getBudgetedLaborCost() {#getBudgetedLaborCost--}
```
public final BigDecimal getBudgetedLaborCost()
```


बजटेड (या नियोजित) श्रम लागत का मान प्राप्त करता है .

**Returns:**
java.math.BigDecimal - बजटेड (या नियोजित) श्रम लागत का मान।
### getBudgetedMaterialCost() {#getBudgetedMaterialCost--}
```
public final BigDecimal getBudgetedMaterialCost()
```


बजटेड (या नियोजित) सामग्री लागत का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - बजटेड (या नियोजित) सामग्री लागत का मान।
### getBudgetedNonlaborCost() {#getBudgetedNonlaborCost--}
```
public final BigDecimal getBudgetedNonlaborCost()
```


बजटेड (या नियोजित) गैर-श्रम लागत का मान प्राप्त करता है .

**Returns:**
java.math.BigDecimal - बजटेड (या नियोजित) गैर-श्रम लागत का मान।
### getBudgetedTotalCost() {#getBudgetedTotalCost--}
```
public final BigDecimal getBudgetedTotalCost()
```


बजटेड (या नियोजित) लागतों का कुल मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - बजटेड (या नियोजित) लागतों का कुल मान।
### getDurationPercentComplete() {#getDurationPercentComplete--}
```
public final double getDurationPercentComplete()
```


अवधि प्रतिशत पूर्णता का मान प्राप्त करता है।

**Returns:**
double - अवधि प्रतिशत पूर्णता का मान।
### getDurationType() {#getDurationType--}
```
public final int getDurationType()
```


गतिविधि के 'Duration Type' फ़ील्ड का मान प्राप्त करता है।

--------------------

केवल गतिविधियों (गैर-सारांश कार्य) के लिए लागू है।

**Returns:**
int - गतिविधि के 'Duration Type' फ़ील्ड का मान।
### getPercentCompleteType() {#getPercentCompleteType--}
```
public final int getPercentCompleteType()
```


गतिविधि के '% Complete Type' फ़ील्ड का मान प्राप्त करता है।

--------------------

केवल गतिविधियों (गैर-सारांश कार्य) के लिए लागू है।

**Returns:**
int - गतिविधि के '% Complete Type' फ़ील्ड का मान।
### getPhysicalPercentComplete() {#getPhysicalPercentComplete--}
```
public final double getPhysicalPercentComplete()
```


भौतिक प्रतिशत पूर्णता का मान प्राप्त करता है।

--------------------

केवल गतिविधियों (गैर-सारांश कार्य) के लिए लागू है।

**Returns:**
double - Physical Percent Complete का मान।
### getPlannedDuration() {#getPlannedDuration--}
```
public final Duration getPlannedDuration()
```


मूल या नियोजित अवधि प्राप्त करता है -- कार्य की नियोजित प्रारंभ तिथि से नियोजित समाप्ति तिथि तक का कुल कार्य समय..

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the original or planned duration -- the total working time from the task planned start date to the planned finish date.
### getPrimaryConstraintDate() {#getPrimaryConstraintDate--}
```
public final Date getPrimaryConstraintDate()
```


प्राथमिक प्रतिबंध की तिथि प्राप्त करता है।

**Returns:**
java.util.Date - प्राथमिक प्रतिबंध की तिथि।
### getPrimaryConstraintType() {#getPrimaryConstraintType--}
```
public final int getPrimaryConstraintType()
```


प्राथमिक प्रतिबंध का प्रकार प्राप्त करता है।

**Returns:**
int - प्राथमिक प्रतिबंध का प्रकार।
### getRawActivityType() {#getRawActivityType--}
```
public final String getRawActivityType()
```


गतिविधि के 'Activity Type' फ़ील्ड का कच्चा पाठ प्रतिनिधित्व (जैसे स्रोत फ़ाइल में) प्राप्त करता है।

--------------------

केवल गतिविधियों (गैर-सारांश कार्य) के लिए लागू है।

**Returns:**
java.lang.String - गतिविधि के 'Activity Type' फ़ील्ड का कच्चा पाठ प्रतिनिधित्व (जैसे स्रोत फ़ाइल में)।
### getRawCompletePercentType() {#getRawCompletePercentType--}
```
public final String getRawCompletePercentType()
```


गतिविधि के '% Complete Type' फ़ील्ड का कच्चा पाठ प्रतिनिधित्व (जैसे स्रोत फ़ाइल में) प्राप्त करता है।

--------------------

केवल गतिविधियों (गैर-सारांश कार्य) के लिए लागू है।

**Returns:**
java.lang.String - गतिविधि के '% Complete Type' फ़ील्ड का कच्चा पाठ प्रतिनिधित्व (जैसे स्रोत फ़ाइल में)।
### getRawDurationType() {#getRawDurationType--}
```
public final String getRawDurationType()
```


गतिविधि के 'Duration Type' फ़ील्ड का कच्चा पाठ प्रतिनिधित्व (जैसे स्रोत फ़ाइल में) प्राप्त करता है।

--------------------

केवल गतिविधियों (गैर-सारांश कार्य) के लिए लागू है।

**Returns:**
java.lang.String - गतिविधि के 'Duration Type' फ़ील्ड का कच्चा पाठ प्रतिनिधित्व (जैसे स्रोत फ़ाइल में)।
### getRawStatus() {#getRawStatus--}
```
public final String getRawStatus()
```


गतिविधि के 'Status' फ़ील्ड का कच्चा पाठ प्रतिनिधित्व (जैसे स्रोत फ़ाइल में) प्राप्त करता है।

--------------------

केवल गतिविधियों (गैर-सारांश कार्य) के लिए लागू है।

**Returns:**
java.lang.String - गतिविधि के 'Status' फ़ील्ड का कच्चा पाठ प्रतिनिधित्व (जैसे स्रोत फ़ाइल में)।
### getRemainingEarlyFinish() {#getRemainingEarlyFinish--}
```
public final Date getRemainingEarlyFinish()
```


शेष प्रारंभिक समाप्ति तिथि प्राप्त करता है - वह तिथि जब गतिविधि के शेष कार्य को समाप्त करने के लिए निर्धारित किया गया है।

**Returns:**
java.util.Date - शेष प्रारंभिक समाप्ति तिथि - वह तिथि जब गतिविधि के शेष कार्य को समाप्त होने के लिए निर्धारित किया गया है।
### getRemainingEarlyStart() {#getRemainingEarlyStart--}
```
public final Date getRemainingEarlyStart()
```


शेष प्रारंभिक प्रारंभ तिथि प्राप्त करता है - वह तिथि जब गतिविधि के शेष कार्य को शुरू करने के लिए निर्धारित किया गया है।

**Returns:**
java.util.Date - शेष प्रारंभिक आरंभ तिथि - वह तिथि जब गतिविधि के शेष कार्य को शुरू होने के लिए निर्धारित किया गया है।
### getRemainingExpenseCost() {#getRemainingExpenseCost--}
```
public final BigDecimal getRemainingExpenseCost()
```


शेष खर्च लागत का मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - शेष व्यय लागत का मान।
### getRemainingLaborUnits() {#getRemainingLaborUnits--}
```
public final double getRemainingLaborUnits()
```


शेष श्रम इकाइयों का मान प्राप्त करता है।

**Returns:**
double - शेष श्रम इकाइयों का मान।
### getRemainingLateFinish() {#getRemainingLateFinish--}
```
public final Date getRemainingLateFinish()
```


शेष देर से समाप्ति तिथि प्राप्त करता है।

**Returns:**
java.util.Date - शेष देर से समाप्ति तिथि।
### getRemainingLateStart() {#getRemainingLateStart--}
```
public final Date getRemainingLateStart()
```


शेष देर से प्रारंभ तिथि प्राप्त करता है।

**Returns:**
java.util.Date - शेष देर से आरंभ तिथि।
### getRemainingNonLaborUnits() {#getRemainingNonLaborUnits--}
```
public final double getRemainingNonLaborUnits()
```


शेष गैर-श्रम इकाइयों का मान प्राप्त करता है।

**Returns:**
double - शेष गैर-श्रम इकाइयों का मान।
### getSecondaryConstraintDate() {#getSecondaryConstraintDate--}
```
public final Date getSecondaryConstraintDate()
```


द्वितीयक प्रतिबंध की तिथि प्राप्त करता है।

**Returns:**
java.util.Date - द्वितीयक प्रतिबंध की तिथि।
### getSecondaryConstraintType() {#getSecondaryConstraintType--}
```
public final int getSecondaryConstraintType()
```


द्वितीयक प्रतिबंध का प्रकार प्राप्त करता है।

**Returns:**
int - द्वितीयक प्रतिबंध का प्रकार।
### getSequenceNumber() {#getSequenceNumber--}
```
public final int getSequenceNumber()
```


WBS आइटम (summary tasks) का क्रमांक प्राप्त करता है। यह Primavera में summary tasks को क्रमबद्ध करने के लिए उपयोग किया जाता है।

--------------------

WBS आइटम (summary tasks) पर लागू।

**Returns:**
int - WBS आइटम (summary tasks) का क्रमांक।
### getUnitsPercentComplete() {#getUnitsPercentComplete--}
```
public final double getUnitsPercentComplete()
```


इकाइयों के प्रतिशत पूर्णता का मान प्राप्त करता है।

**Returns:**
double - इकाइयों के प्रतिशत पूर्णता का मान।
