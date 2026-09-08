---
title: "Project.Resources"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Возвращает объект ResourceCollection"
type: docs
weight: 780
url: /ru/net/aspose.tasks/project/resources/
---
## Project.Resources property

Получает объект ResourceCollection.

```csharp
public ResourceCollection Resources { get; }
```

## Примеры

Показывает, как создавать ресурсы проекта.

```csharp
public void CreateResources()
{
    var project = new Project(DataDir + "project-sort.mpp");

    // Добавить ресурс
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

### См. также

* class [ResourceCollection](../../resourcecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


