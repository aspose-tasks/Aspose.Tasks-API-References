---
title: "Κλάση ListUtils"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Util.ListUtils. Κλάση βοηθητικού προγράμματος για επεξεργασία λιστών"
type: docs
weight: 2740
url: /el/net/aspose.tasks.util/listutils/
---
## ListUtils class

Κλάση βοηθητικού προγράμματος για επεξεργασία λιστών.

```csharp
public static class ListUtils
```

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| static [Apply&lt;T&gt;](../../aspose.tasks.util/listutils/apply/)(IList&lt;T&gt;, IAlgorithm&lt;T&gt;, int) | Εφαρμόστε τον αλγόριθμο για κάθε στοιχείο λίστας ξεκινώντας από τη συγκεκριμένη θέση. |
| static [Filter&lt;T&gt;](../../aspose.tasks.util/listutils/filter/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | Φιλτράρετε τα στοιχεία της λίστας με βάση την καθορισμένη συνθήκη. |
| static [Find&lt;T&gt;](../../aspose.tasks.util/listutils/find/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | Βρείτε την πρώτη εμφάνιση ενός στοιχείου λίστας που ικανοποιεί την καθορισμένη συνθήκη. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τη μέθοδο Find του εργαλείου λίστας.

```csharp
public void WorkWithListUtilsFind()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> taskFilters = project.TaskFilters.ToList();

    Assert.AreEqual(3, taskFilters.Count, "Project.TaskFilters count");

    var filter = ListUtils.Find(taskFilters, new FilterByName("&All Tasks"));

    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Filter Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

public class FilterByName : ICondition<Filter>
{
    private readonly string name;

    public FilterByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// Επιστρέφει true εάν το συγκεκριμένο αντικείμενο ικανοποιεί τις συνθήκες.
    /// </summary>
    /// <param name="el">Το αντικείμενο προς έλεγχο.</param>
    /// <returns>True εάν το αντικείμενο ικανοποιεί τις συνθήκες.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Name == this.name;
    }
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


