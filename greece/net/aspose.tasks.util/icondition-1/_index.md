---
title: "Διεπαφή IConditionT"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Util.ICondition1T διεπαφή. Αντιπροσωπεύει μια συνθήκη που μπορεί να χρησιμοποιηθεί από φίλτρα ή μεθόδους αναζήτησης"
type: docs
weight: 2720
url: /el/net/aspose.tasks.util/icondition-1/
---
## ICondition&lt;T&gt; interface

Αναπαριστά μια συνθήκη που μπορεί να χρησιμοποιηθεί από φίλτρα ή μεθόδους αναζήτησης.

```csharp
public interface ICondition<in T>
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | Ο τύπος του αντικειμένου στο οποίο θα εφαρμοστεί η διεπαφή μεθόδου. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Check](../../aspose.tasks.util/icondition-1/check/)(T) | Επιστρέφει true εάν το καθορισμένο αντικείμενο ικανοποιεί τις συνθήκες. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


