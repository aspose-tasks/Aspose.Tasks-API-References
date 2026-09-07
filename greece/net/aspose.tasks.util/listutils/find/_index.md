---
title: "ListUtils.Find"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ListUtils μέθοδος. Βρίσκει την πρώτη εμφάνιση ενός στοιχείου λίστας που ικανοποιεί την καθορισμένη συνθήκη"
type: docs
weight: 30
url: /el/net/aspose.tasks.util/listutils/find/
---
## ListUtils.Find&lt;T&gt; method

Βρείτε την πρώτη εμφάνιση ενός στοιχείου λίστας που ικανοποιεί την καθορισμένη συνθήκη.

```csharp
public static T Find<T>(IList<T> list, ICondition<T> cond)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | Ο τύπος του αντικειμένου προς εύρεση. |
| λίστα | Μια λίστα προς επεξεργασία. |
| cond | Συνθήκη που χρησιμοποιείται για την εύρεση ενός στοιχείου στην καθορισμένη λίστα. |

### Τιμή Επιστροφής

Στοιχείο λίστας ή null.

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


