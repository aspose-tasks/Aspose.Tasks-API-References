---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupTaskDefinition method"
linktitle: "CreateLookupTaskDefinition"
articleTitle: "CreateLookupTaskDefinition"
second_title: "Aspose.Tasks C++ के लिए"
description: "फ़ैक्टरी मेथड जो लुकअप के साथ एक विस्तारित गुण परिभाषा बनाता है।"
type: docs
weight: 40
url: /hi/cpp/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---

## CreateLookupTaskDefinition (1 of 2) {#createlookuptaskdefinition_1}

लुकअप के साथ एक विस्तारित गुण परिभाषा बनाने वाली फ़ैक्टरी मेथड। इसमें CalculationType Tasks::CalculationType::Lookup के बराबर है और यह केवल Tasks में उपयोग की जा सकती है। जब इस मेथड को कॉल करते हैं तो आपको customFieldType , fieldId और alias निर्दिष्ट करने की आवश्यकता है।

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| पैरामीटर | विवरण |
| --- | --- |
| customFieldType | निर्दिष्ट CustomFieldType प्रकार। |
| fieldId | निर्दिष्ट ExtendedAttributeTask फ़ील्ड ID। |
| alias | निर्दिष्ट System::String उपनाम। |

---

## CreateLookupTaskDefinition (2 of 2) {#createlookuptaskdefinition_2}

फ़ैक्टरी मेथड जो लुकअप के साथ एक विस्तारित एट्रिब्यूट परिभाषा बनाता है। इसका CalculationType Tasks::CalculationType::Lookup के बराबर है और इसे केवल Tasks में उपयोग किया जा सकता है। इस मेथड को कॉल करते समय आपको fieldId और alias निर्दिष्ट करना आवश्यक है। फ़ील्ड प्रकार field id से अनुमानित किया जाता है।

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| पैरामीटर | विवरण |
| --- | --- |
| fieldId | निर्दिष्ट ExtendedAttributeTask फ़ील्ड ID। |
| alias | निर्दिष्ट System::String उपनाम। |

