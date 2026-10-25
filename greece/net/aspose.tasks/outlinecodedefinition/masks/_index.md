---
title: "OutlineCodeDefinition.Masks"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "OutlineCodeDefinition ιδιότητα. Λαμβάνει το αντικείμενο OutlineMaskCollection. Ο πίνακας των καταχωρίσεων που ορίζουν τη μάσκα κώδικα περιγράμματος. Αντικείμενο OutlineMaskCollection μόνο για ανάγνωση"
type: docs
weight: 100
url: /el/net/aspose.tasks/outlinecodedefinition/masks/
---
## OutlineCodeDefinition.Masks property

Λαμβάνει το αντικείμενο OutlineMaskCollection. Ο πίνακας των καταχωρίσεων που ορίζουν τη μάσκα κώδικα περιγράμματος. Μόνο για ανάγνωση [`OutlineMaskCollection`](../../outlinemaskcollection/) instance.

```csharp
public OutlineMaskCollection Masks { get; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με ορισμούς outline code.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// δημιουργήστε έναν νέο ορισμό outline code
var outline = new OutlineCodeDefinition();

// ορίστε τον αριθμό πεδίου ενός outline code
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");

// ορίστε το όνομα ενός προσαρμοσμένου outline code
outline.FieldName = "Outline Code1";

// ορίστε το Guid ενός outline code
outline.Guid = "e6afac06-0d86-4359-a96c-db705e3d2ca8";

// ορίστε μια τιμή που υποδεικνύει εάν οι τιμές που καθορίζονται σε αυτό το πεδίο outline code πρέπει να είναι τιμές φύλλου
outline.LeafOnly = false;

// ορίστε το ψευδώνυμο ενός προσαρμοσμένου outline code
outline.Alias = "My Outline Code";

// ορίστε την φωνητική προφορά του ψευδώνυμου του προσαρμοσμένου outline code
outline.PhoneticAlias = "Outline Code";

// ορίστε μια τιμή που υποδεικνύει εάν οι νέοι κώδικες πρέπει να έχουν όλα τα επίπεδα. Δεν είναι διαθέσιμο για Enterprise Codes.
outline.AllLevelsRequired = true;

// ορίστε μια τιμή που υποδεικνύει εάν ένας προσαρμοσμένος outline code είναι enterprise custom outline code
outline.Enterprise = false;

// ορίστε μια αναφορά σε άλλο προσαρμοσμένο πεδίο για το οποίο αυτός ο ορισμός outline code είναι ψευδώνυμο
outline.EnterpriseOutlineCodeAlias = 0;

// προσθέστε μια outline mask
var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// ορίστε μια τιμή που υποδεικνύει εάν οι καθορισμένες τιμές πρέπει να προέρχονται από τον πίνακα τιμών
outline.OnlyTableValuesAllowed = false;

// ορίστε μια τιμή που υποδεικνύει εάν ο προσαρμοσμένος outline code μπορεί να χρησιμοποιηθεί
// από το Resource Substitution Wizard στο Microsoft Project
outline.ResourceSubstitutionEnabled = false;

// ορίστε μια τιμή που υποδεικνύει εάν τα εσοχές αυτού του outline code πρέπει να εμφανίζονται.
outline.ShowIndent = false;

project.OutlineCodes.Add(outline);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### Δείτε επίσης

* class [OutlineMaskCollection](../../outlinemaskcollection/)
* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


