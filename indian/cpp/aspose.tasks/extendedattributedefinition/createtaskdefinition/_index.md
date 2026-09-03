---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateTaskDefinition method"
linktitle: "CreateTaskDefinition"
articleTitle: "CreateTaskDefinition"
second_title: "Aspose.Tasks C++ के लिए"
description: "फ़ैक्टरी मेथड जो एक सरल विस्तारित एट्रिब्यूट परिभाषा बनाता है, जिसे Microsoft Project \"None\" के रूप में दिखाता है।"
type: docs
weight: 60
url: /hi/cpp/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---

## CreateTaskDefinition (1 of 2) {#createtaskdefinition_1}

सरल विस्तारित गुण परिभाषा बनाने वाली फ़ैक्टरी मेथड, जिसे Microsoft Project "None" के रूप में दिखाता है। इसमें CalculationType Tasks::CalculationType::None के बराबर है और यह केवल Tasks में उपयोग की जा सकती है। जब इस मेथड को कॉल किया जाता है तो आपको customFieldType , fieldId और alias निर्दिष्ट करने की आवश्यकता है।

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| पैरामीटर | विवरण |
| --- | --- |
| customFieldType | निर्दिष्ट CustomFieldType प्रकार। |
| fieldId | निर्दिष्ट ExtendedAttributeTask फ़ील्ड ID। |
| alias | निर्दिष्ट System::String उपनाम। |

---

## CreateTaskDefinition (2 of 2) {#createtaskdefinition_2}

फ़ैक्टरी मेथड जो एक सरल विस्तारित एट्रिब्यूट परिभाषा बनाता है, जिसे Microsoft Project "None" के रूप में दिखाता है। इसका CalculationType Tasks::CalculationType::None के बराबर है और इसे केवल Tasks में उपयोग किया जा सकता है। इस मेथड को कॉल करते समय आपको fieldId और alias निर्दिष्ट करना आवश्यक है। फ़ील्ड प्रकार field id से अनुमानित किया जाता है।

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| पैरामीटर | विवरण |
| --- | --- |
| fieldId | निर्दिष्ट ExtendedAttributeTask फ़ील्ड ID। |
| alias | निर्दिष्ट System::String उपनाम। |

