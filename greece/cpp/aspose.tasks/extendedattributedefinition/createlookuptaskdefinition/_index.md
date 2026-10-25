---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupTaskDefinition μέθοδος"
linktitle: "CreateLookupTaskDefinition"
articleTitle: "CreateLookupTaskDefinition"
second_title: "Aspose.Tasks για C++"
description: "Μέθοδος κατασκευής που δημιουργεί έναν ορισμό εκτεταμένου χαρακτηριστικού με αναζήτηση."
type: docs
weight: 40
url: /el/cpp/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---

## CreateLookupTaskDefinition (1 of 2) {#createlookuptaskdefinition_1}

Μέθοδος κατασκευής που δημιουργεί έναν ορισμό εκτεταμένου χαρακτηριστικού με αναζήτηση. Έχει CalculationType ίσο με Tasks::CalculationType::Lookup και μπορεί να χρησιμοποιηθεί μόνο σε Tasks. Απαιτείται να καθορίσετε customFieldType, fieldId και alias όταν καλείτε αυτή τη μέθοδο.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| customFieldType | Ο καθορισμένος τύπος CustomFieldType. |
| fieldId | Το καθορισμένο αναγνωριστικό πεδίου ExtendedAttributeTask. |
| alias | Το καθορισμένο ψευδώνυμο System::String. |

---

## CreateLookupTaskDefinition (2 of 2) {#createlookuptaskdefinition_2}

Μέθοδος κατασκευής που δημιουργεί έναν ορισμό εκτεταμένου χαρακτηριστικού με αναζήτηση. Έχει CalculationType ίσο με Tasks::CalculationType::Lookup και μπορεί να χρησιμοποιηθεί μόνο σε Tasks. Απαιτείται να καθορίσετε το fieldId και το alias όταν καλείτε αυτή τη μέθοδο. Ο τύπος του πεδίου προκύπτει από το field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| fieldId | Το καθορισμένο αναγνωριστικό πεδίου ExtendedAttributeTask. |
| alias | Το καθορισμένο ψευδώνυμο System::String. |

