---
title: "Κλάση Filter"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Filter. Αντιπροσωπεύει ένα φίλτρο στο Project"
type: docs
weight: 600
url: /el/net/aspose.tasks/filter/
---
## Filter class

Αντιπροσωπεύει ένα φίλτρο στο Project.

```csharp
public sealed class Filter : IComparable<Filter>, IEquatable<Filter>
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Filter](filter/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Criteria](../../aspose.tasks/filter/criteria/) { get; set; } | Λαμβάνει ή ορίζει τα κριτήρια που πρέπει να πληρούν οι εργασίες ή οι πόροι για να εμφανιστούν στην προβολή MSP. |
| [FilterType](../../aspose.tasks/filter/filtertype/) { get; set; } | Λαμβάνει τον τύπο του φίλτρου. |
| [Index](../../aspose.tasks/filter/index/) { get; } | Λαμβάνει το δείκτη ενός αντικειμένου `Filter` στο αντικείμενο που περιέχει τα Filters. |
| [Name](../../aspose.tasks/filter/name/) { get; set; } | Λαμβάνει ή ορίζει το όνομα ενός αντικειμένου Filter. |
| [ShowInMenu](../../aspose.tasks/filter/showinmenu/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το έργο εμφανίζει το όνομα του φίλτρου στη λίστα επιλογής Filter στην καρτέλα Προβολή της κορδέλας. |
| [ShowRelatedSummaryRows](../../aspose.tasks/filter/showrelatedsummaryrows/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν εμφανίζονται σχετικές γραμμές σύνοψης για το φίλτρο. |
| [Uid](../../aspose.tasks/filter/uid/) { get; } | Λαμβάνει το μοναδικό αναγνωριστικό ενός φίλτρου. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [CompareTo](../../aspose.tasks/filter/compareto/)(Filter) | Συγκρίνει αυτή την παρουσία με την καθορισμένη παρουσία της κλάσης `Filter` και επιστρέφει μια ένδειξη της σχετικής τους σειράς. |
| [Equals](../../aspose.tasks/filter/equals/#equals)(Filter) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο AssignmentBaseline. |
| override [Equals](../../aspose.tasks/filter/equals/#equals_1)(object) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο AssignmentBaseline. |
| override [GetHashCode](../../aspose.tasks/filter/gethashcode/)() | Επιστρέφει μια τιμή κώδικα κατακερματισμού για το φίλτρο. |
| [operator ==](../../aspose.tasks/filter/op_equality/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [operator &gt;](../../aspose.tasks/filter/op_greaterthan/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη από ένα καθορισμένο αντικείμενο. |
| [operator &gt;=](../../aspose.tasks/filter/op_greaterthanorequal/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη ή ίση με ένα καθορισμένο αντικείμενο. |
| [operator !=](../../aspose.tasks/filter/op_inequality/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο. |
| [operator &lt;](../../aspose.tasks/filter/op_lessthan/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη από ένα καθορισμένο αντικείμενο. |
| [operator &lt;=](../../aspose.tasks/filter/op_lessthanorequal/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη ή ίση με ένα καθορισμένο αντικείμενο. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με φίλτρα.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();
Console.WriteLine("Task filters count: " + filters.Count);
foreach (var filter in filters)
{
    Console.WriteLine("Uid: " + filter.Uid);
    Console.WriteLine("Index: " + filter.Index);
    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

// ελέγξτε τα φίλτρα πόρων
List<Filter> resourceFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + resourceFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + resourceFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + resourceFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + resourceFilters[0].ShowRelatedSummaryRows);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


