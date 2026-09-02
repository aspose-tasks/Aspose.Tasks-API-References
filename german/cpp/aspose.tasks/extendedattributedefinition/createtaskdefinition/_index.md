---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateTaskDefinition Methode"
linktitle: "CreateTaskDefinition"
articleTitle: "CreateTaskDefinition"
second_title: "Aspose.Tasks für C++"
description: "Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als \\\"None\\\" anzeigt."
type: docs
weight: 60
url: /de/cpp/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---

## CreateTaskDefinition (1 of 2) {#createtaskdefinition_1}

Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. Sie hat CalculationType gleich zu Tasks::CalculationType::None und kann nur in Tasks verwendet werden. Sie müssen customFieldType , fieldId und alias angeben, wenn Sie diese Methode aufrufen.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parameter | Beschreibung |
| --- | --- |
| customFieldType | Der angegebene CustomFieldType-Typ. |
| fieldId | Die angegebene ExtendedAttributeTask-Feld-ID. |
| alias | Der angegebene System::String-Alias. |

---

## CreateTaskDefinition (2 of 2) {#createtaskdefinition_2}

Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als \"None\" anzeigt. Sie hat CalculationType gleich Tasks::CalculationType::None und kann nur in Tasks verwendet werden. Sie müssen fieldId und alias angeben, wenn Sie diese Methode aufrufen. Der Feldtyp wird aus der field id abgeleitet.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parameter | Beschreibung |
| --- | --- |
| fieldId | Die angegebene ExtendedAttributeTask-Feld-ID. |
| alias | Der angegebene System::String-Alias. |

