---
title: "NullableBool.ToString"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος NullableBool. Επιστρέφει μια συμβολοσειρά που αντιπροσωπεύει το τρέχον αντικείμενο."
type: docs
weight: 60
url: /el/net/aspose.tasks/nullablebool/tostring/
---
## NullableBool.ToString method

Επιστρέφει μια συμβολοσειρά που αντιπροσωπεύει το τρέχον αντικείμενο.

```csharp
public override string ToString()
```

### Τιμή Επιστροφής

Μια συμβολοσειρά που αντιπροσωπεύει το τρέχον αντικείμενο.

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


