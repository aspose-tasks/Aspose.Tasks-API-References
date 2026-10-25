---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateResourceDefinition methode"
linktitle: "CreateResourceDefinition"
articleTitle: "CreateResourceDefinition"
second_title: "Aspose.Tasks voor C++"
description: "Factory-methode die een eenvoudige uitgebreide attribuutdefinitie maakt, die Microsoft Project weergeeft als \"None\"."
type: docs
weight: 50
url: /nl/cpp/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---

## CreateResourceDefinition (1 of 2) {#createresourcedefinition_1}

Factory-methode die een eenvoudige definitie van een uitgebreid attribuut maakt, die Microsoft Project weergeeft als "None". Deze heeft CalculationType gelijk aan Tasks::CalculationType::None en kan alleen in Resource worden gebruikt. U moet customFieldType, fieldId en alias opgeven bij het aanroepen van deze methode.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parameter | Beschrijving |
| --- | --- |
| customFieldType | Het opgegeven CustomFieldType‑type. |
| fieldId | De opgegeven ExtendedAttributeResource‑veld‑ID. |
| alias | De opgegeven System::String‑alias. |

---

## CreateResourceDefinition (2 of 2) {#createresourcedefinition_2}

Factory-methode die een eenvoudige uitgebreide attribuutdefinitie maakt, die Microsoft Project weergeeft als "None". Het heeft CalculationType gelijk aan Tasks::CalculationType::None en kan alleen in Resource worden gebruikt. U moet fieldId en alias opgeven bij het aanroepen van deze methode. Het veldtype wordt afgeleid van field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parameter | Beschrijving |
| --- | --- |
| fieldId | De opgegeven ExtendedAttributeResource‑veld‑ID. |
| alias | De opgegeven System::String‑alias. |

