---
title: "Κλάση OutlineValue"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.OutlineValue. Αντιπροσωπεύει μια τιμή περιγράμματος"
type: docs
weight: 1210
url: /el/net/aspose.tasks/outlinevalue/
---
## OutlineValue class

Αντιπροσωπεύει μια τιμή περίγραμμα.

```csharp
public class OutlineValue
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [OutlineValue](outlinevalue/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Description](../../aspose.tasks/outlinevalue/description/) { get; set; } | Λαμβάνει ή ορίζει την περιγραφή μιας τιμής περιγράμματος. |
| [DurationValue](../../aspose.tasks/outlinevalue/durationvalue/) { get; set; } | Λαμβάνει ή ορίζει τη διάρκεια εάν ο Τύπος είναι Duration. |
| [IsCollapsed](../../aspose.tasks/outlinevalue/iscollapsed/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν η τιμή περιγράμματος είναι συμπτυγμένη ή όχι. |
| [ParentValueId](../../aspose.tasks/outlinevalue/parentvalueid/) { get; set; } | Λαμβάνει ή ορίζει το Id ενός γονικού κόμβου ενός κώδικα περιγράμματος. |
| [Type](../../aspose.tasks/outlinevalue/type/) { get; set; } | Λαμβάνει ή ορίζει τον τύπο κώδικα περιγράμματος. |
| [Value](../../aspose.tasks/outlinevalue/value/) { get; set; } | Λαμβάνει ή ορίζει την πραγματική τιμή. |
| [ValueGuid](../../aspose.tasks/outlinevalue/valueguid/) { get; } | Λαμβάνει ένα GUID που αναγνωρίζει αυτήν την τιμή μεταξύ των άλλων σε ολόκληρο το έργο. |
| [ValueId](../../aspose.tasks/outlinevalue/valueid/) { get; set; } | Λαμβάνει ή ορίζει το μοναδικό Id μιας τιμής κώδικα περιγράμματος εντός ενός έργου. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τιμές περιγράμματος.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";
var outline2 = new OutlineCodeDefinition();
outline2.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline2.Alias = "My Outline Code 2";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// δημιουργήστε μια τιμή περιγράμματος
var value = new OutlineValue();

// ορίστε την πραγματική τιμή
value.Value = "Text value 1";

// ορίστε το μοναδικό Id μιας τιμής κώδικα περιγράμματος μέσα σε ένα έργο
value.ValueId = 1;

// λάβετε ένα GUID που αναγνωρίζει αυτή την τιμή μεταξύ των άλλων σε ολόκληρο το έργο
Console.WriteLine("Check value GUID: " + value.ValueGuid);

// ορίστε τον τύπο κώδικα περιγράμματος
value.Type = OutlineValueType.Text;

// ορίστε την περιγραφή μιας τιμής περιγράμματος
value.Description = "Text value descr 1";

// ορίστε μια τιμή που υποδεικνύει εάν η τιμή περιγράμματος είναι συμπτυγμένη ή όχι
value.IsCollapsed = false;

// ελέγξτε το id της γονικής τιμής
Console.WriteLine("Check parent value id: " + value.ParentValueId);
outline.Values.Add(value);

// δημιουργήστε μια τιμή περιγράμματος με διάρκεια
var value2 = new OutlineValue();

// ορίστε την τιμή διάρκειας
value2.DurationValue = project.GetDuration(1, TimeUnitType.Hour);

// ορίστε το μοναδικό Id μιας τιμής κώδικα περιγράμματος μέσα σε ένα έργο
value2.ValueId = 2;
outline2.Values.Add(value2);

// ...
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


