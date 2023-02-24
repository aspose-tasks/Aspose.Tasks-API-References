---
title: CreateResourceDefinition
second_title: Aspose.Tasks για Αναφορά API .NET
description: Εργοστασιακή μέθοδος που δημιουργεί έναν απλό εκτεταμένο ορισμό χαρακτηριστικών τον οποίο το Microsoft Project εμφανίζει ως Κανένα. ΈχειCalculationTypeaspose.tasks/extendedattributedefinition/calculationtype/ Ισούται μεNone και μπορεί να χρησιμοποιηθεί μόνο σε πόρους. Πρέπει να καθορίσετεcustomFieldType fieldId καιalias όταν καλείτε αυτήν τη μέθοδο.
type: docs
weight: 30
url: /el/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Εργοστασιακή μέθοδος που δημιουργεί έναν απλό εκτεταμένο ορισμό χαρακτηριστικών, τον οποίο το Microsoft Project εμφανίζει ως "Κανένα". Έχει[`CalculationType`](../calculationtype/) Ισούται μεNone και μπορεί να χρησιμοποιηθεί μόνο σε πόρους. Πρέπει να καθορίσετε*customFieldType* ,*fieldId* και*alias* όταν καλείτε αυτήν τη μέθοδο.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| customFieldType | CustomFieldType | Το καθορισμένο[`CustomFieldType`](../../customfieldtype/) τύπος. |
| fieldId | ExtendedAttributeResource | Το καθορισμένο[`ExtendedAttributeResource`](../../extendedattributeresource/) αναγνωριστικό πεδίου. |
| alias | String | Το καθορισμένοString ψευδώνυμο. |

### Επιστρεφόμενη Αξία

Δημιουργήθηκε το παράδειγμα του[`ExtendedAttributeDefinition`](../) τάξη με καθορισμένο*customFieldType* ,*fieldId* και*alias*.

### Παραδείγματα

Χρησιμοποιήστε αυτό το παράδειγμα για να δημιουργήσετε έναν προσαρμοσμένο ορισμό πεδίου κειμένου:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Δείτε επίσης

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* χώρος ονομάτων [Aspose.Tasks](../../extendedattributedefinition/)
* συνέλευση [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Εργοστασιακή μέθοδος που δημιουργεί έναν απλό εκτεταμένο ορισμό χαρακτηριστικών, τον οποίο το Microsoft Project εμφανίζει ως "Κανένα". Έχει[`CalculationType`](../calculationtype/) Ισούται μεNone και μπορεί να χρησιμοποιηθεί μόνο σε πόρους. Πρέπει να καθορίσετε*fieldId* και*alias* όταν καλείτε αυτήν τη μέθοδο. Ο τύπος πεδίου προκύπτει από το πεδίο id.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Το καθορισμένο[`ExtendedAttributeResource`](../../extendedattributeresource/) αναγνωριστικό πεδίου. |
| alias | String | Το καθορισμένοString ψευδώνυμο. |

### Επιστρεφόμενη Αξία

Δημιουργήθηκε το παράδειγμα του[`ExtendedAttributeDefinition`](../) τάξη με καθορισμένο*fieldId* και*alias*.

### Παραδείγματα

Χρησιμοποιήστε αυτό το παράδειγμα για να δημιουργήσετε έναν προσαρμοσμένο ορισμό πεδίου κειμένου:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Δείτε επίσης

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* χώρος ονομάτων [Aspose.Tasks](../../extendedattributedefinition/)
* συνέλευση [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->