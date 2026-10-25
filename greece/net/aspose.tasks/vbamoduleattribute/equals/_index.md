---
title: "VbaModuleAttribute.Equals"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος VbaModuleAttribute. Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο VbaModuleAttribute"
type: docs
weight: 30
url: /el/net/aspose.tasks/vbamoduleattribute/equals/
---
## Equals(VbaModuleAttribute) {#equals}

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο [`VbaModuleAttribute`](../).

```csharp
public bool Equals(VbaModuleAttribute other)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | VbaModuleAttribute | Το καθορισμένο αντικείμενο [`VbaModuleAttribute`](../) για σύγκριση με αυτή την παρουσία. |

### Τιμή Επιστροφής

Επιστρέφει true εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο [`VbaModuleAttribute`](../); διαφορετικά, false.

## Παραδείγματα

Δείχνει πώς να ελέγξετε την ισότητα των ιδιοτήτων μονάδας VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### Δείτε επίσης

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο [`VbaModuleAttribute`](../).

```csharp
public override bool Equals(object obj)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | Object | Το καθορισμένο αντικείμενο [`VbaModuleAttribute`](../) για σύγκριση με αυτή την παρουσία. |

### Τιμή Επιστροφής

Επιστρέφει true εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο [`VbaModuleAttribute`](../); διαφορετικά, false.

## Παραδείγματα

Δείχνει πώς να ελέγξετε την ισότητα των ιδιοτήτων μονάδας VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### Δείτε επίσης

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


