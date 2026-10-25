---
title: "ExtendedAttribute.FlagValue"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ExtendedAttribute. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν έχει οριστεί σημαία για μια ιδιότητα τύπου Flag"
type: docs
weight: 50
url: /el/net/aspose.tasks/extendedattribute/flagvalue/
---
## ExtendedAttribute.FlagValue property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν έχει οριστεί σημαία για χαρακτηριστικό τύπου 'Flag'.

```csharp
public bool FlagValue { get; set; }
```

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Εκτοπίζεται εάν η ιδιότητα [`AttributeDefinition`](../attributedefinition/) δεν έχει αρχικοποιηθεί ή η τρέχουσα ιδιότητα δεν είναι ιδιότητα σημαίας. |

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε μια boolean εκτεταμένη ιδιότητα.

```csharp
var project = new Project();

// δημιουργήστε νέο ορισμό επεκτατικού χαρακτηριστικού εργασίας
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Flag, ExtendedAttributeTask.Flag1, "Is Finished");

// Προσθέστε έναν τύπο στην ιδιότητα.
definition.Formula = "[% Complete] = 100";

project.ExtendedAttributes.Add(definition);

var finished = project.RootTask.Children.Add("Task");
finished.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
finished.Set(Tsk.ActualStart, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.ActualDuration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.ActualFinish, new DateTime(2020, 4, 21, 17, 0, 0));
finished.Set(Tsk.PercentComplete, 100);

var running = project.RootTask.Children.Add("Task");
running.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
running.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
running.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
running.Set(Tsk.ActualStart, new DateTime(2020, 4, 21, 8, 0, 0));

Console.WriteLine(running.Get(Tsk.PercentComplete));
// δημιουργήστε εκτεταμένη ιδιότητα
var runningFlagAttribute = definition.CreateExtendedAttribute();
var finishedFlagAttribute = definition.CreateExtendedAttribute();
running.ExtendedAttributes.Add(runningFlagAttribute);
finished.ExtendedAttributes.Add(finishedFlagAttribute);

Console.WriteLine("Alias: {0}\n", definition.Alias);
Console.WriteLine("(Finished Task) Field Id: " + finishedFlagAttribute.FieldId);
Console.WriteLine("(Finished Task) Value: {0}\n", finishedFlagAttribute.FlagValue);
Console.WriteLine("(Running Task) Field Id: " + runningFlagAttribute.FieldId);
Console.WriteLine("(Running Task) Value: " + runningFlagAttribute.FlagValue);
```

### Δείτε επίσης

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


