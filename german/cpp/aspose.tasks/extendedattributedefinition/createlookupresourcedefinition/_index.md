---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupResourceDefinition Methode"
linktitle: "CreateLookupResourceDefinition"
articleTitle: "CreateLookupResourceDefinition"
second_title: "Aspose.Tasks für C++"
description: "Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt."
type: docs
weight: 30
url: /de/cpp/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---

## CreateLookupResourceDefinition (1 of 2) {#createlookupresourcedefinition_1}

Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. Sie hat CalculationType gleich zu Tasks::CalculationType::Lookup und kann nur in Resources verwendet werden. Sie müssen customFieldType , fieldId und alias angeben, wenn Sie diese Methode aufrufen.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parameter | Beschreibung |
| --- | --- |
| customFieldType | Der angegebene CustomFieldType-Typ. |
| fieldId | Die angegebene ExtendedAttributeResource-Feld-ID. |
| alias | Der angegebene System::String-Alias. |

---

## CreateLookupResourceDefinition (2 of 2) {#createlookupresourcedefinition_2}

Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. Sie hat CalculationType gleich Tasks::CalculationType::Lookup und kann nur in Resources verwendet werden. Sie müssen fieldId und alias angeben, wenn Sie diese Methode aufrufen. Der Feldtyp wird aus der field id abgeleitet.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parameter | Beschreibung |
| --- | --- |
| fieldId | Die angegebene ExtendedAttributeResource-Feld-ID. |
| alias | Der angegebene System::String-Alias. |

