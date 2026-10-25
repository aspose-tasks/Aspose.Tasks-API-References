---
title: "Klasse ListUtils"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Util.ListUtils klasse. Utilityklasse voor lijstverwerking"
type: docs
weight: 2740
url: /nl/net/aspose.tasks.util/listutils/
---
## ListUtils class

Hulpprogrammaklasse voor lijstverwerking.

```csharp
public static class ListUtils
```

## Methoden

| Naam | Beschrijving |
| --- | --- |
| static [Apply&lt;T&gt;](../../aspose.tasks.util/listutils/apply/)(IList&lt;T&gt;, IAlgorithm&lt;T&gt;, int) | Pas het algoritme toe op elk lijstelement beginnend vanaf de opgegeven positie. |
| static [Filter&lt;T&gt;](../../aspose.tasks.util/listutils/filter/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | Filter lijstelementen op basis van de opgegeven voorwaarde. |
| static [Find&lt;T&gt;](../../aspose.tasks.util/listutils/find/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | Vind de eerste keer dat een lijstelement voldoet aan de opgegeven voorwaarde. |

## Voorbeelden

Toont hoe te werken met de Find-methode van list util.

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
    /// Retourneert true als het opgegeven object aan de voorwaarden voldoet.
    /// </summary>
    /// <param name=\"el\">Het object om te controleren.</param>
    /// <returns>True als het object aan de voorwaarden voldoet.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Name == this.name;
    }
}
```

### Zie ook

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


