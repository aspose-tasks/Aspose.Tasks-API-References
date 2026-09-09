---
title: "Project.Resources"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. ResourceCollection nesnesini alır."
type: docs
weight: 780
url: /tr/net/aspose.tasks/project/resources/
---
## Project.Resources property

ResourceCollection nesnesini alır.

```csharp
public ResourceCollection Resources { get; }
```

## Örnekler

Proje kaynaklarını nasıl oluşturacağınızı gösterir.

```csharp
public void CreateResources()
{
    var project = new Project(DataDir + "project-sort.mpp");

    // Bir kaynak ekle
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

### Ayrıca Bakınız

* class [ResourceCollection](../../resourcecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


