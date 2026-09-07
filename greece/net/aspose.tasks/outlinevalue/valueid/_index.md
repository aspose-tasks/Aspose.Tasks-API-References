---
title: "OutlineValue.ValueId"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα OutlineValue. Λαμβάνει ή ορίζει το μοναδικό Id μιας τιμής κώδικα περιγράμματος μέσα σε ένα έργο"
type: docs
weight: 90
url: /el/net/aspose.tasks/outlinevalue/valueid/
---
## OutlineValue.ValueId property

Λαμβάνει ή ορίζει το μοναδικό Id μιας τιμής κώδικα περιγράμματος εντός ενός έργου.

```csharp
public int ValueId { get; set; }
```

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

* class [OutlineValue](../)
* namespace [Aspose.Tasks](../../outlinevalue/)
* assembly [Aspose.Tasks](../../../)


