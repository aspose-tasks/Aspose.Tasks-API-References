---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateResourceDefinition Methode"
linktitle: "CreateResourceDefinition"
articleTitle: "CreateResourceDefinition"
second_title: "Aspose.Tasks für C++"
description: "Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als \\\"None\\\" anzeigt."
type: docs
weight: 50
url: /de/cpp/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---

## CreateResourceDefinition (1 of 2) {#createresourcedefinition_1}

Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. Sie hat CalculationType gleich zu Tasks::CalculationType::None und kann nur in Resource verwendet werden. Sie müssen customFieldType , fieldId und alias angeben, wenn Sie diese Methode aufrufen.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parameter | Beschreibung |
| --- | --- |
| customFieldType | Der angegebene CustomFieldType-Typ. |
| fieldId | Die angegebene ExtendedAttributeResource-Feld-ID. |
| alias | Der angegebene System::String-Alias. |

---

## CreateResourceDefinition (2 of 2) {#createresourcedefinition_2}

Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. Sie hat CalculationType gleich zu Tasks::CalculationType::None und kann nur in Resource verwendet werden. Sie müssen fieldId und alias angeben, wenn Sie diese Methode aufrufen. Der Feldtyp wird aus field id abgeleitet.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parameter | Beschreibung |
| --- | --- |
| fieldId | Die angegebene ExtendedAttributeResource-Feld-ID. |
| alias | Der angegebene System::String-Alias. |

