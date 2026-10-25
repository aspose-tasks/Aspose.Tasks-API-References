---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupResourceDefinition μέθοδος"
linktitle: "CreateLookupResourceDefinition"
articleTitle: "CreateLookupResourceDefinition"
second_title: "Aspose.Tasks για C++"
description: "Μέθοδος κατασκευής που δημιουργεί έναν ορισμό εκτεταμένου χαρακτηριστικού με αναζήτηση."
type: docs
weight: 30
url: /el/cpp/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---

## CreateLookupResourceDefinition (1 of 2) {#createlookupresourcedefinition_1}

Μέθοδος κατασκευής που δημιουργεί έναν ορισμό εκτεταμένου χαρακτηριστικού με αναζήτηση. Έχει CalculationType ίσο με Tasks::CalculationType::Lookup και μπορεί να χρησιμοποιηθεί μόνο σε Resources. Απαιτείται να καθορίσετε customFieldType, fieldId και alias όταν καλείτε αυτή τη μέθοδο.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| customFieldType | Ο καθορισμένος τύπος CustomFieldType. |
| fieldId | Το καθορισμένο αναγνωριστικό πεδίου ExtendedAttributeResource. |
| alias | Το καθορισμένο ψευδώνυμο System::String. |

---

## CreateLookupResourceDefinition (2 of 2) {#createlookupresourcedefinition_2}

Μέθοδος κατασκευής που δημιουργεί έναν ορισμό εκτεταμένου χαρακτηριστικού με αναζήτηση. Έχει CalculationType ίσο με Tasks::CalculationType::Lookup και μπορεί να χρησιμοποιηθεί μόνο σε Resources. Απαιτείται να καθορίσετε το fieldId και το alias όταν καλείτε αυτή τη μέθοδο. Ο τύπος του πεδίου προκύπτει από το field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| fieldId | Το καθορισμένο αναγνωριστικό πεδίου ExtendedAttributeResource. |
| alias | Το καθορισμένο ψευδώνυμο System::String. |

