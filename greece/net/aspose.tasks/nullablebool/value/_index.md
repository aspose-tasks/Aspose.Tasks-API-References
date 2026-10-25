---
title: "NullableBool.Value"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα NullableBool. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν η τρέχουσα τιμή είναι true ή false."
type: docs
weight: 30
url: /el/net/aspose.tasks/nullablebool/value/
---
## NullableBool.Value property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η τρέχουσα τιμή είναι true ή false.

```csharp
public bool Value { get; set; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με την κλάση &lt;see cref=\"NullableBool\" /&gt;.

```csharp
var project = new Project();

// Ας ελέγξουμε πού χρησιμοποιείται η κλάση <see cref=\"Aspose.Tasks.NullableBool\" />.
// Το κύριο πλεονέκτημα της <see cref=\"Aspose.Tasks.NullableBool\" /> είναι ότι 
// Μπορεί κανείς να το ορίσει ως ακαθόριστο μέσω δημιουργίας
var actualsInSync = new NullableBool(false, false);
Console.WriteLine("'ActualsInSync' Value: " + actualsInSync.Value);
Console.WriteLine("'ActualsInSync' Is Defined: " + actualsInSync.IsDefined);

// ...
// χρησιμοποιήστε ένα αντικείμενο nullable bool
project.Set(Prj.ActualsInSync, actualsInSync);

// ...
var honorConstraints = new NullableBool(true);
Console.WriteLine("'HonorConstraints' ToString: " + honorConstraints.ToString());

// ...
// χρησιμοποιήστε ένα αντικείμενο nullable bool
project.Set(Prj.HonorConstraints, honorConstraints);

// ...
```

### Δείτε επίσης

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


