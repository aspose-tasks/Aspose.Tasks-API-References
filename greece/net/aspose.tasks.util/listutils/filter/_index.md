---
title: "ListUtils.Filter"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ListUtils μέθοδος. Φιλτράρει στοιχεία λίστας με την καθορισμένη συνθήκη"
type: docs
weight: 20
url: /el/net/aspose.tasks.util/listutils/filter/
---
## ListUtils.Filter&lt;T&gt; method

Φιλτράρετε τα στοιχεία της λίστας με βάση την καθορισμένη συνθήκη.

```csharp
public static IList<T> Filter<T>(IList<T> list, ICondition<T> cond)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | Ο τύπος του αντικειμένου στο οποίο θα εφαρμοστεί το φίλτρο. |
| λίστα | Μια λίστα προς επεξεργασία. |
| cond | Συνθήκη που χρησιμοποιείται για το φιλτράρισμα της καθορισμένης λίστας. |

### Τιμή Επιστροφής

Φιλτραρισμένη λίστα.

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τη μέθοδο Filter της λίστας util.

```csharp
public void WorkWithListUtilsFilter()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> filters = project.TaskFilters.ToList();

    Assert.AreEqual(3, filters.Count, "Project.TaskFilters count");

    ListUtils.Filter(filters, new FilterByIndex(1));

    foreach (var filter in filters)
    {
        Console.WriteLine("Name: " + filter.Name);
        Console.WriteLine("Filter Type: " + filter.FilterType);
        Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
        Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
        Console.WriteLine();
    }
}

public class FilterByIndex : ICondition<Filter>
{
    private readonly int index;

    public FilterByIndex(int index)
    {
        this.index = index;
    }

    /// <summary>
    /// Επιστρέφει true εάν το συγκεκριμένο αντικείμενο ικανοποιεί τις συνθήκες.
    /// </summary>
    /// <param name="el">Το αντικείμενο προς έλεγχο.</param>
    /// <returns>True εάν το αντικείμενο ικανοποιεί τις συνθήκες.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Index == this.index;
    }
}
```

### Δείτε επίσης

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


