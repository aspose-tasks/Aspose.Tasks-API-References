---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateResourceDefinition मेथड"
linktitle: "CreateResourceDefinition"
articleTitle: "CreateResourceDefinition"
second_title: "Aspose.Tasks C++ के लिए"
description: "फ़ैक्टरी मेथड जो एक सरल विस्तारित एट्रिब्यूट परिभाषा बनाता है, जिसे Microsoft Project \"None\" के रूप में दिखाता है।"
type: docs
weight: 50
url: /hi/cpp/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---

## CreateResourceDefinition (1 of 2) {#createresourcedefinition_1}

सरल विस्तारित गुण परिभाषा बनाने वाली फ़ैक्टरी मेथड, जिसे Microsoft Project "None" के रूप में दिखाता है। इसमें CalculationType Tasks::CalculationType::None के बराबर है और यह केवल Resource में उपयोग की जा सकती है। जब इस मेथड को कॉल करते हैं तो आपको customFieldType , fieldId और alias निर्दिष्ट करने की आवश्यकता है।

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| पैरामीटर | विवरण |
| --- | --- |
| customFieldType | निर्दिष्ट CustomFieldType प्रकार। |
| fieldId | निर्दिष्ट ExtendedAttributeResource फ़ील्ड आईडी। |
| alias | निर्दिष्ट System::String उपनाम। |

---

## CreateResourceDefinition (2 of 2) {#createresourcedefinition_2}

एक फ़ैक्टरी मेथड जो एक सरल विस्तारित गुण परिभाषा बनाता है, जिसे Microsoft Project "None" के रूप में दिखाता है। इसका CalculationType Tasks::CalculationType::None के बराबर है और इसे केवल Resource में उपयोग किया जा सकता है। इस मेथड को कॉल करते समय आपको fieldId और alias निर्दिष्ट करना आवश्यक है। फ़ील्ड प्रकार field id से अनुमानित किया जाता है।

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| पैरामीटर | विवरण |
| --- | --- |
| fieldId | निर्दिष्ट ExtendedAttributeResource फ़ील्ड आईडी। |
| alias | निर्दिष्ट System::String उपनाम। |

