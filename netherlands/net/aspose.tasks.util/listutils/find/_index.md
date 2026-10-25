---
title: "ListUtils.Find"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ListUtils-methode. Zoek de eerste voorkoming van een lijstonderdeel dat voldoet aan de opgegeven voorwaarde"
type: docs
weight: 30
url: /nl/net/aspose.tasks.util/listutils/find/
---
## ListUtils.Find&lt;T&gt; method

Vind de eerste keer dat een lijstelement voldoet aan de opgegeven voorwaarde.

```csharp
public static T Find<T>(IList<T> list, ICondition<T> cond)
```

| Parameter | Beschrijving |
| --- | --- |
| T | Het type object om te vinden. |
| lijst | Een lijst om te verwerken. |
| cond | Voorwaarde die wordt gebruikt om een element in de opgegeven lijst te vinden. |

### Retourwaarde

Lijstelement of null.

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


