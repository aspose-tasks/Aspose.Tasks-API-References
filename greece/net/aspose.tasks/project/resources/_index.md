---
title: "Project.Resources"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει το αντικείμενο ResourceCollection"
type: docs
weight: 780
url: /el/net/aspose.tasks/project/resources/
---
## Project.Resources property

Λαμβάνει το αντικείμενο ResourceCollection.

```csharp
public ResourceCollection Resources { get; }
```

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε πόρους έργου.

```csharp
public void CreateResources()
{
    var project = new Project(DataDir + "project-sort.mpp");

    // Προσθέστε έναν πόρο
    project.Resources.Add("Rsc");

    List<Resource> resources = project.Resources.ToList();
    resources.Sort(new RscNameComparer());

    foreach (var rsc in resources)
    {
        Console.WriteLine(rsc);
    }

    project.Save(OutDir + "CreateResources_out.xml", SaveFileFormat.Xml);
}

private class RscNameComparer : IComparer<Resource>
{
    public int Compare(Resource x, Resource y)
    {
        if (x == null && y == null)
        {
            return 0;
        }

        if (x == null)
        {
            return -1;
        }

        if (y == null)
        {
            return 1;
        }

        if (string.IsNullOrEmpty(x.Get(Rsc.Name)))
        {
            return 1;
        }

        if (string.IsNullOrEmpty(y.Get(Rsc.Name)))
        {
            return -1;
        }

        return string.Compare(x.Get(Rsc.Name), y.Get(Rsc.Name), StringComparison.Ordinal);
    }
}
```

### Δείτε επίσης

* class [ResourceCollection](../../resourcecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


