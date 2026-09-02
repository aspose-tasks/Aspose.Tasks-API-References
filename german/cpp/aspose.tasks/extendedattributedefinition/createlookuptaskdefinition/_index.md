---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupTaskDefinition Methode"
linktitle: "CreateLookupTaskDefinition"
articleTitle: "CreateLookupTaskDefinition"
second_title: "Aspose.Tasks für C++"
description: "Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt."
type: docs
weight: 40
url: /de/cpp/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---

## CreateLookupTaskDefinition (1 of 2) {#createlookuptaskdefinition_1}

Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. Sie hat CalculationType gleich zu Tasks::CalculationType::Lookup und kann nur in Tasks verwendet werden. Sie müssen customFieldType , fieldId und alias angeben, wenn Sie diese Methode aufrufen.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parameter | Beschreibung |
| --- | --- |
| customFieldType | Der angegebene CustomFieldType-Typ. |
| fieldId | Die angegebene ExtendedAttributeTask-Feld-ID. |
| alias | Der angegebene System::String-Alias. |

---

## CreateLookupTaskDefinition (2 of 2) {#createlookuptaskdefinition_2}

Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. Sie hat CalculationType gleich Tasks::CalculationType::Lookup und kann nur in Tasks verwendet werden. Sie müssen fieldId und alias angeben, wenn Sie diese Methode aufrufen. Der Feldtyp wird aus der field id abgeleitet.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parameter | Beschreibung |
| --- | --- |
| fieldId | Die angegebene ExtendedAttributeTask-Feld-ID. |
| alias | Der angegebene System::String-Alias. |

