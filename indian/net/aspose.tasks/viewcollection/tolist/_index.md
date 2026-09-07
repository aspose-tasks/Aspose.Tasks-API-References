---
title: "ViewCollection.ToList"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ViewCollection मेथड। एक व्यू संग्रह को View ऑब्जेक्ट्स की सूची में परिवर्तित करता है"
type: docs
weight: 120
url: /hi/net/aspose.tasks/viewcollection/tolist/
---
## ViewCollection.ToList method

एक व्यू संग्रह को [`View`](../../view/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है।

```csharp
public List<View> ToList()
```

### रिटर्न वैल्यू

[`View`](../../view/) ऑब्जेक्ट्स की जेनेरिक सूची।

## उदाहरण

दिखाता है कि view संग्रहों के साथ कैसे काम करें।

```csharp
var project = new Project(DataDir + "Project1.mpp");

// view की साधारण सूची में बदलें
List<View> list = project.Views.ToList();
for (var index = 0; index < list.Count; index++)
{
    var viewToChange = list[index];
    viewToChange.PageInfo.Header.CenteredText = "Header " + index;
}

// एक नया view जोड़ें
var view = new GanttChartView();
if (!project.Views.IsReadOnly)
{
    project.Views.Add(view);
}

// view पर इटरेट करें
Console.WriteLine("Iterate over views of " + project.Views.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Project view count: " + project.Views.Count);
Console.WriteLine();
foreach (var projectView in project.Views)
{
    Console.WriteLine("Name: " + projectView.Name);
}

// सभी view एक साथ हटाएँ
project.Views.Clear();

// या एक-एक करके
{
    // पद्धति 1
    List<View> listToDelete = project.Views.ToList();
    foreach (var v in listToDelete)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}

{
    // पद्धति 2
    var array = new View[project.Views.Count];
    project.Views.CopyTo(array, 0);
    foreach (var v in array)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}
```

### संबंधित देखें

* class [View](../../view/)
* class [ViewCollection](../)
* namespace [Aspose.Tasks](../../viewcollection/)
* assembly [Aspose.Tasks](../../../)


