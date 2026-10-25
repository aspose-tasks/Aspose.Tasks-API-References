---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupResourceDefinition method"
linktitle: "CreateLookupResourceDefinition"
articleTitle: "CreateLookupResourceDefinition"
second_title: "Aspose.Tasks voor C++"
description: "Factory‑methode die een definitie van een uitgebreid attribuut met opzoekfunctie maakt."
type: docs
weight: 30
url: /nl/cpp/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---

## CreateLookupResourceDefinition (1 of 2) {#createlookupresourcedefinition_1}

Factory-methode die een definitie van een uitgebreid attribuut met opzoekfunctie maakt. Deze heeft CalculationType gelijk aan Tasks::CalculationType::Lookup en kan alleen in Resources worden gebruikt. U moet customFieldType, fieldId en alias opgeven bij het aanroepen van deze methode.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parameter | Beschrijving |
| --- | --- |
| customFieldType | Het opgegeven CustomFieldType‑type. |
| fieldId | De opgegeven ExtendedAttributeResource‑veld‑ID. |
| alias | De opgegeven System::String‑alias. |

---

## CreateLookupResourceDefinition (2 of 2) {#createlookupresourcedefinition_2}

Factory-methode die een uitgebreide attribuutdefinitie met lookup maakt. Deze heeft CalculationType gelijk aan Tasks::CalculationType::Lookup en kan alleen in Resources worden gebruikt. U moet fieldId en alias opgeven bij het aanroepen van deze methode. Het veldtype wordt afgeleid van field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parameter | Beschrijving |
| --- | --- |
| fieldId | De opgegeven ExtendedAttributeResource‑veld‑ID. |
| alias | De opgegeven System::String‑alias. |

