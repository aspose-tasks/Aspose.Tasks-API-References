---
title: "Filter.Equals"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Filter. Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσίαση είναι ίση με το καθορισμένο αντικείμενο AssignmentBaseline."
type: docs
weight: 100
url: /el/net/aspose.tasks/filter/equals/
---
## Equals(Filter) {#equals}

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο AssignmentBaseline.

```csharp
public bool Equals(Filter other)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| άλλο | Filter | το καθορισμένο αντικείμενο AssignmentBaseline για σύγκριση με αυτήν την παρουσίαση. |

### Τιμή Επιστροφής

επιστρέφει true εάν αυτή η παρουσίαση είναι ίση με το καθορισμένο αντικείμενο AssignmentBaseline; διαφορετικά, false.

## Παραδείγματα

Δείχνει πώς να ελέγξετε την ισότητα των φίλτρων.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();

var filter1 = filters[0];
var filter2 = filters[1];

// η ισότητα των φίλτρων ελέγχεται σε σχέση με το UID του φίλτρου.
Console.WriteLine("Filter 1 UID: " + filter1.Uid);
Console.WriteLine("Filter 2 UID: " + filter2.Uid);
Console.WriteLine("Are filters equal: " + filter1.Equals(filter2));
```

### Δείτε επίσης

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο AssignmentBaseline.

```csharp
public override bool Equals(object obj)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | Αντικείμενο | το καθορισμένο αντικείμενο AssignmentBaseline για σύγκριση με αυτήν την παρουσίαση. |

### Τιμή Επιστροφής

επιστρέφει true εάν αυτή η παρουσίαση είναι ίση με το καθορισμένο αντικείμενο AssignmentBaseline; διαφορετικά, false.

## Παραδείγματα

Δείχνει πώς να ελέγξετε την ισότητα των φίλτρων.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();

var filter1 = filters[0];
var filter2 = filters[1];

// η ισότητα των φίλτρων ελέγχεται σε σχέση με το UID του φίλτρου.
Console.WriteLine("Filter 1 UID: " + filter1.Uid);
Console.WriteLine("Filter 2 UID: " + filter2.Uid);
Console.WriteLine("Are filters equal: " + filter1.Equals(filter2));
```

### Δείτε επίσης

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


