---
title: "Διεπαφή IAlgorithmT"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Διεπαφή Aspose.Tasks.Util.IAlgorithm1T. Αντιπροσωπεύει έναν αλγόριθμο που μπορεί να εφαρμοστεί σε μια λίστα αντικειμένων T"
type: docs
weight: 2710
url: /el/net/aspose.tasks.util/ialgorithm-1/
---
## IAlgorithm&lt;T&gt; interface

Αναπαριστά έναν αλγόριθμο που μπορεί να εφαρμοστεί σε μια λίστα αντικειμένων *T*.

```csharp
public interface IAlgorithm<in T>
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | Ο τύπος του αντικειμένου στο οποίο θα εφαρμοστεί η διεπαφή μεθόδου. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Alg](../../aspose.tasks.util/ialgorithm-1/alg/)(T, int) | Επεξεργάζεται ένα αντικείμενο στη λίστα. Καλείται μετά το [`PreAlg`](./prealg/); |
| [PostAlg](../../aspose.tasks.util/ialgorithm-1/postalg/)(T, int) | Καλείται μετά την επεξεργασία ενός αντικειμένου. |
| [PreAlg](../../aspose.tasks.util/ialgorithm-1/prealg/)(T, int) | Καλείται πριν από την επεξεργασία ενός αντικειμένου. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


