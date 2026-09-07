---
title: "Filter.op_GreaterThan"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Filter. Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη από ένα καθορισμένο αντικείμενο"
type: docs
weight: 130
url: /el/net/aspose.tasks/filter/op_greaterthan/
---
## Filter GreaterThan operator

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη από ένα καθορισμένο αντικείμενο.

```csharp
public static bool operator >(Filter a, Filter b)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| α | Filter | Το πρώτο φίλτρο. |
| β | Filter | Το δεύτερο φίλτρο. |

### Τιμή Επιστροφής

μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη από ένα καθορισμένο αντικείμενο

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


