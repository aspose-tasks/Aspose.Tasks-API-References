---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateTaskDefinition methode"
linktitle: "CreateTaskDefinition"
articleTitle: "CreateTaskDefinition"
second_title: "Aspose.Tasks voor C++"
description: "Factory-methode die een eenvoudige uitgebreide attribuutdefinitie maakt, die Microsoft Project weergeeft als \"None\"."
type: docs
weight: 60
url: /nl/cpp/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---

## CreateTaskDefinition (1 of 2) {#createtaskdefinition_1}

Factory-methode die een eenvoudige definitie van een uitgebreid attribuut maakt, die Microsoft Project weergeeft als "None". Deze heeft CalculationType gelijk aan Tasks::CalculationType::None en kan alleen in Tasks worden gebruikt. U moet customFieldType, fieldId en alias opgeven bij het aanroepen van deze methode.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parameter | Beschrijving |
| --- | --- |
| customFieldType | Het opgegeven CustomFieldType‑type. |
| fieldId | Het opgegeven ExtendedAttributeTask veld-ID. |
| alias | De opgegeven System::String‑alias. |

---

## CreateTaskDefinition (2 of 2) {#createtaskdefinition_2}

Factory-methode die een eenvoudige uitgebreide attribuutdefinitie maakt, die Microsoft Project weergeeft als "None". Deze heeft CalculationType gelijk aan Tasks::CalculationType::None en kan alleen in Tasks worden gebruikt. U moet fieldId en alias opgeven bij het aanroepen van deze methode. Het veldtype wordt afgeleid van field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parameter | Beschrijving |
| --- | --- |
| fieldId | Het opgegeven ExtendedAttributeTask veld-ID. |
| alias | De opgegeven System::String‑alias. |

