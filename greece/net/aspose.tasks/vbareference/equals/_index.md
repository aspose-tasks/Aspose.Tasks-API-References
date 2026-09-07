---
title: "VbaReference.Equals"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος VbaReference. Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο VbaReference"
type: docs
weight: 40
url: /el/net/aspose.tasks/vbareference/equals/
---
## Equals(VbaReference) {#equals}

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο [`VbaReference`](../).

```csharp
public bool Equals(VbaReference other)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | VbaReference | Το καθορισμένο αντικείμενο [`VbaReference`](../) για σύγκριση με αυτήν την παρουσία. |

### Τιμή Επιστροφής

Επιστρέφει true εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο [`VbaReference`](../); διαφορετικά, false.

## Παραδείγματα

Δείχνει πώς να ελέγξετε την ισότητα της αναφοράς VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// Η ισότητα των αναφορών ελέγχεται με βάση το όνομα της αναφοράς.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### Δείτε επίσης

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο [`VbaReference`](../).

```csharp
public override bool Equals(object obj)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | Object | Το καθορισμένο αντικείμενο [`VbaReference`](../) για σύγκριση με αυτήν την παρουσία. |

### Τιμή Επιστροφής

Επιστρέφει true εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο [`VbaReference`](../); διαφορετικά, false.

## Παραδείγματα

Δείχνει πώς να ελέγξετε την ισότητα της αναφοράς VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// Η ισότητα των αναφορών ελέγχεται με βάση το όνομα της αναφοράς.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### Δείτε επίσης

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


