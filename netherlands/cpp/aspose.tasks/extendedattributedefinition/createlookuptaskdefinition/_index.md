---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupTaskDefinition methode"
linktitle: "CreateLookupTaskDefinition"
articleTitle: "CreateLookupTaskDefinition"
second_title: "Aspose.Tasks voor C++"
description: "Factory‑methode die een definitie van een uitgebreid attribuut met opzoekfunctie maakt."
type: docs
weight: 40
url: /nl/cpp/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---

## CreateLookupTaskDefinition (1 of 2) {#createlookuptaskdefinition_1}

Factory-methode die een definitie van een uitgebreid attribuut met opzoekfunctie maakt. Deze heeft CalculationType gelijk aan Tasks::CalculationType::Lookup en kan alleen in Tasks worden gebruikt. U moet customFieldType, fieldId en alias opgeven bij het aanroepen van deze methode.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parameter | Beschrijving |
| --- | --- |
| customFieldType | Het opgegeven CustomFieldType‑type. |
| fieldId | Het opgegeven ExtendedAttributeTask veld-ID. |
| alias | De opgegeven System::String‑alias. |

---

## CreateLookupTaskDefinition (2 of 2) {#createlookuptaskdefinition_2}

Factory-methode die een uitgebreide attribuutdefinitie met lookup maakt. Deze heeft CalculationType gelijk aan Tasks::CalculationType::Lookup en kan alleen in Tasks worden gebruikt. U moet fieldId en alias opgeven bij het aanroepen van deze methode. Het veldtype wordt afgeleid van field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parameter | Beschrijving |
| --- | --- |
| fieldId | Het opgegeven ExtendedAttributeTask veld-ID. |
| alias | De opgegeven System::String‑alias. |

