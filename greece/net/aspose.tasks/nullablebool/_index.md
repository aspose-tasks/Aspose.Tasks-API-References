---
title: "Δομή NullableBool"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.NullableBool struct. Μια κλάση για λογικές τιμές με δυνατότητα έλεγχου εάν η τιμή ορίστηκε ή όχι."
type: docs
weight: 1110
url: /el/net/aspose.tasks/nullablebool/
---
## NullableBool structure

Μια κλάση για λογικές τιμές με δυνατότητα ελέγχου εάν η τιμή έχει οριστεί ή όχι.

```csharp
public struct NullableBool : IEquatable<NullableBool>
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [NullableBool](nullablebool/#constructor)(bool) | Αρχικοποιεί μια νέα παρουσία της δομής `NullableBool` με την καθορισμένη λογική τιμή. |
| [NullableBool](nullablebool/#constructor_1)(bool, bool) | Αρχικοποιεί μια νέα παρουσία της δομής `NullableBool`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [IsDefined](../../aspose.tasks/nullablebool/isdefined/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν η τιμή ορίστηκε· διαφορετικά, false. |
| [Value](../../aspose.tasks/nullablebool/value/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η τρέχουσα τιμή είναι true ή false. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Equals](../../aspose.tasks/nullablebool/equals/#equals)(NullableBool) | Επιστρέφει μια σημαία που υποδεικνύει εάν αυτή η παρουσία είναι ίση με την καθορισμένη παρουσία της κλάσης `NullableBool`. |
| override [Equals](../../aspose.tasks/nullablebool/equals/#equals_1)(object) | Επιστρέφει μια σημαία που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο. |
| override [GetHashCode](../../aspose.tasks/nullablebool/gethashcode/)() | Επιστρέφει μια τιμή κώδικα κατακερματισμού για την παρουσία της κλάσης `NullableBool`. |
| override [ToString](../../aspose.tasks/nullablebool/tostring/)() | Επιστρέφει μια συμβολοσειρά που αντιπροσωπεύει το τρέχον αντικείμενο. |
| [operator ==](../../aspose.tasks/nullablebool/op_equality/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [implicit operator](../../aspose.tasks/nullablebool/op_implicit/#op_implicit_1) | Μετατρέπει έμμεσα ένα αντικείμενο `NullableBool` σε τιμή boolean. Επιστρέφει true όταν το [`Value`](./value/) είναι true και το [`IsDefined`](./isdefined/) είναι true. (2 τελεστές) |
| [operator !=](../../aspose.tasks/nullablebool/op_inequality/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


