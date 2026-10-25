---
title: "NullableBool.NullableBool"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής NullableBool. Αρχικοποιεί μια νέα παρουσία της δομής NullableBool με την καθορισμένη τιμή boolean."
type: docs
weight: 10
url: /el/net/aspose.tasks/nullablebool/nullablebool/
---
## NullableBool(bool) {#constructor}

Αρχικοποιεί μια νέα παρουσία της δομής [`NullableBool`](../) με την καθορισμένη τιμή boolean.

```csharp
public NullableBool(bool value)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | Boolean | η καθορισμένη λογική τιμή. |

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

---

## NullableBool(bool, bool) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του δομικού τύπου [`NullableBool`](../).

```csharp
public NullableBool(bool value, bool isDefined)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | Boolean | Η τρέχουσα τιμή. |
| isDefined | Boolean | Η τιμή που υποδεικνύει αν η τρέχουσα τιμή είναι ορισμένη. |

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


