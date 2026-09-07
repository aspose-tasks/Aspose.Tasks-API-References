---
title: "ICondition1.Check"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ICondition. Επιστρέφει true εάν το συγκεκριμένο αντικείμενο ικανοποιεί τις συνθήκες"
type: docs
weight: 10
url: /el/net/aspose.tasks.util/icondition-1/check/
---
## ICondition&lt;T&gt;.Check method

Επιστρέφει true εάν το καθορισμένο αντικείμενο ικανοποιεί τις συνθήκες.

```csharp
public bool Check(T el)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | T | Το αντικείμενο προς έλεγχο. |

### Τιμή Επιστροφής

Αληθές εάν το αντικείμενο ικανοποιεί τις προϋποθέσεις.

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

* interface [ICondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../icondition-1/)
* assembly [Aspose.Tasks](../../../)


