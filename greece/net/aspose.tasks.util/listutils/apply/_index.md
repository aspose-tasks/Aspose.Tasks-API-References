---
title: "ListUtils.Apply"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ListUtils μέθοδος. Εφαρμόζει αλγόριθμο για κάθε στοιχείο λίστας ξεκινώντας από τη καθορισμένη θέση"
type: docs
weight: 10
url: /el/net/aspose.tasks.util/listutils/apply/
---
## ListUtils.Apply&lt;T&gt; method

Εφαρμόστε τον αλγόριθμο για κάθε στοιχείο λίστας ξεκινώντας από τη συγκεκριμένη θέση.

```csharp
public static void Apply<T>(IList<T> list, IAlgorithm<T> algorithm, int startIndex)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | Ο τύπος του αντικειμένου στον οποίο θα εφαρμοστεί ο αλγόριθμος. |
| λίστα | Λίστα προς επεξεργασία. |
| αλγόριθμος | Εφαρμοσμένος αλγόριθμος. |
| startIndex | Θέση αρχικού στοιχείου. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τη μέθοδο Apply της λίστας util.

```csharp
public void WorkWithListUtilsApply()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> filters = project.TaskFilters.ToList();

    Assert.AreEqual(3, filters.Count, "Project.TaskFilters count");

    ListUtils.Apply(filters, new RenameAlgorithm(), 0);

    foreach (var filter in filters)
    {
        Console.WriteLine("Name: " + filter.Name);
        Console.WriteLine("Filter Type: " + filter.FilterType);
        Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
        Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
        Console.WriteLine();
    }
}

private class RenameAlgorithm : IAlgorithm<Filter>
{
    private int current;

    public RenameAlgorithm()
    {
        this.current = 0;
    }

    public void PreAlg(Filter el, int index)
    {
        this.current++;
    }

    public void Alg(Filter el, int index)
    {
        el.Name = el.Name + " " + this.current;
    }

    public void PostAlg(Filter el, int index)
    {
    }
}
```

### Δείτε επίσης

* interface [IAlgorithm&lt;T&gt;](../../ialgorithm-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


