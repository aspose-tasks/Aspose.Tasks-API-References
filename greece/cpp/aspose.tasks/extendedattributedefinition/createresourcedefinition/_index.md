---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateResourceDefinition μέθοδος"
linktitle: "CreateResourceDefinition"
articleTitle: "CreateResourceDefinition"
second_title: "Aspose.Tasks για C++"
description: "Μέθοδος κατασκευής που δημιουργεί έναν απλό ορισμό εκτεταμένου χαρακτηριστικού, ο οποίος εμφανίζεται στο Microsoft Project ως \"None\"."
type: docs
weight: 50
url: /el/cpp/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---

## CreateResourceDefinition (1 of 2) {#createresourcedefinition_1}

Μέθοδος κατασκευής που δημιουργεί έναν απλό ορισμό εκτεταμένου χαρακτηριστικού, ο οποίος εμφανίζεται στο Microsoft Project ως "None". Έχει CalculationType ίσο με Tasks::CalculationType::None και μπορεί να χρησιμοποιηθεί μόνο σε Resource. Απαιτείται να καθορίσετε customFieldType, fieldId και alias όταν καλείτε αυτή τη μέθοδο.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| customFieldType | Ο καθορισμένος τύπος CustomFieldType. |
| fieldId | Το καθορισμένο αναγνωριστικό πεδίου ExtendedAttributeResource. |
| alias | Το καθορισμένο ψευδώνυμο System::String. |

---

## CreateResourceDefinition (2 of 2) {#createresourcedefinition_2}

Μέθοδος κατασκευής που δημιουργεί έναν απλό ορισμό εκτεταμένου χαρακτηριστικού, ο οποίος εμφανίζεται στο Microsoft Project ως "None". Έχει CalculationType ίσο με Tasks::CalculationType::None και μπορεί να χρησιμοποιηθεί μόνο σε Resource. Απαιτείται να καθορίσετε το fieldId και το alias όταν καλείτε αυτή τη μέθοδο. Ο τύπος του πεδίου προκύπτει από το field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| fieldId | Το καθορισμένο αναγνωριστικό πεδίου ExtendedAttributeResource. |
| alias | Το καθορισμένο ψευδώνυμο System::String. |

