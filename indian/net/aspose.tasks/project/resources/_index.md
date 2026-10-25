---
title: "Project.Resources"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। ResourceCollection ऑब्जेक्ट प्राप्त करता है"
type: docs
weight: 780
url: /hi/net/aspose.tasks/project/resources/
---
## Project.Resources property

ResourceCollection ऑब्जेक्ट प्राप्त करता है।

```csharp
public ResourceCollection Resources { get; }
```

## उदाहरण

प्रोजेक्ट संसाधन बनाने का तरीका दिखाता है।

```csharp
public void CreateResources()
{
    var project = new Project(DataDir + "project-sort.mpp");

    // एक संसाधन जोड़ें
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

### संबंधित देखें

* class [ResourceCollection](../../resourcecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


