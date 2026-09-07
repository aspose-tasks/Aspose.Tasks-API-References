---
title: "Filter.CompareTo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Filter. Συγκρίνει αυτήν την παρουσίαση με την καθορισμένη παρουσίαση της κλάσης Filter και επιστρέφει ένδειξη της σχετικής τους σειράς."
type: docs
weight: 90
url: /el/net/aspose.tasks/filter/compareto/
---
## Filter.CompareTo method

Συγκρίνει αυτήν την παρουσίαση με την καθορισμένη παρουσίαση της κλάσης [`Filter`](../) και επιστρέφει ένδειξη της σχετικής τους σειράς.

```csharp
public int CompareTo(Filter other)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | Filter | την καθορισμένη παρουσίαση της κλάσης [`Filter`](../) για σύγκριση με αυτό το αντικείμενο. |

### Τιμή Επιστροφής

μία ένδειξη της σχετικής τους σειράς.

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


