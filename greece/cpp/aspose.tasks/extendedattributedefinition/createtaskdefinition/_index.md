---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateTaskDefinition μέθοδος"
linktitle: "CreateTaskDefinition"
articleTitle: "CreateTaskDefinition"
second_title: "Aspose.Tasks για C++"
description: "Μέθοδος κατασκευής που δημιουργεί έναν απλό ορισμό εκτεταμένου χαρακτηριστικού, ο οποίος εμφανίζεται στο Microsoft Project ως \"None\"."
type: docs
weight: 60
url: /el/cpp/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---

## CreateTaskDefinition (1 of 2) {#createtaskdefinition_1}

Μέθοδος κατασκευής που δημιουργεί έναν απλό ορισμό εκτεταμένου χαρακτηριστικού, ο οποίος εμφανίζεται στο Microsoft Project ως "None". Έχει CalculationType ίσο με Tasks::CalculationType::None και μπορεί να χρησιμοποιηθεί μόνο σε Tasks. Απαιτείται να καθορίσετε customFieldType, fieldId και alias όταν καλείτε αυτή τη μέθοδο.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| customFieldType | Ο καθορισμένος τύπος CustomFieldType. |
| fieldId | Το καθορισμένο αναγνωριστικό πεδίου ExtendedAttributeTask. |
| alias | Το καθορισμένο ψευδώνυμο System::String. |

---

## CreateTaskDefinition (2 of 2) {#createtaskdefinition_2}

Μέθοδος κατασκευής που δημιουργεί έναν απλό ορισμό εκτεταμένου χαρακτηριστικού, ο οποίος εμφανίζεται στο Microsoft Project ως "None". Έχει CalculationType ίσο με Tasks::CalculationType::None και μπορεί να χρησιμοποιηθεί μόνο σε Tasks. Απαιτείται να καθορίσετε το fieldId και το alias όταν καλείτε αυτή τη μέθοδο. Ο τύπος του πεδίου προκύπτει από το field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| fieldId | Το καθορισμένο αναγνωριστικό πεδίου ExtendedAttributeTask. |
| alias | Το καθορισμένο ψευδώνυμο System::String. |

