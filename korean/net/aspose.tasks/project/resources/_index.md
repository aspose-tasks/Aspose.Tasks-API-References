---
title: "Project.Resources"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. ResourceCollection 객체를 가져옵니다."
type: docs
weight: 780
url: /ko/net/aspose.tasks/project/resources/
---
## Project.Resources property

ResourceCollection 객체를 가져옵니다.

```csharp
public ResourceCollection Resources { get; }
```

## 예제

프로젝트 리소스를 만드는 방법을 보여줍니다.

```csharp
public void CreateResources()
{
    var project = new Project(DataDir + "project-sort.mpp");

    // 리소스 추가
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

### 또 보기

* class [ResourceCollection](../../resourcecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


