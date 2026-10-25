---
title: "IAlgorithm1.PreAlg"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος IAlgorithm. Καλείται πριν από την επεξεργασία ενός αντικειμένου"
type: docs
weight: 30
url: /el/net/aspose.tasks.util/ialgorithm-1/prealg/
---
## IAlgorithm&lt;T&gt;.PreAlg method

Καλείται πριν από την επεξεργασία ενός αντικειμένου.

```csharp
public void PreAlg(T el, int index)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | T | Αντικείμενο που επεξεργάστηκε. |
| index | Int32 | Δείκτης του αντικειμένου. |

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

* interface [IAlgorithm&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../ialgorithm-1/)
* assembly [Aspose.Tasks](../../../)


