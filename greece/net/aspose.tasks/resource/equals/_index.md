---
title: "Resource.Equals"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Resource. Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με μια καθορισμένη παρουσία της κλάσης Resource"
type: docs
weight: 820
url: /el/net/aspose.tasks/resource/equals/
---
## Equals(Resource) {#equals}

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με μια καθορισμένη παρουσία της κλάσης [`Resource`](../).

```csharp
public bool Equals(Resource other)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | Resource | Η καθορισμένη παρουσία της κλάσης [`Resource`](../) για σύγκριση με αυτήν την παρουσία. |

### Τιμή Επιστροφής

**True** if the specified instance of the [`Resource`](../) class has the same Uid value as this instance; otherwise, **false**.

## Παραδείγματα

Δείχνει πώς να ελέγξετε την ισότητα των πόρων.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### Δείτε επίσης

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

```csharp
public override bool Equals(object obj)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | Αντικείμενο | Το αντικείμενο για σύγκριση με αυτήν την παρουσία. |

### Τιμή Επιστροφής

**True** if the specified object is a Resource that has the same Uid value as this instance; otherwise, **false**.

## Παραδείγματα

Δείχνει πώς να ελέγξετε την ισότητα των πόρων.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### Δείτε επίσης

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


