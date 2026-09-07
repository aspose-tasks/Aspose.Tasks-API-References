---
title: "ViewCollection.CopyTo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ViewCollection मेथड। इस संग्रह के तत्वों को निर्दिष्ट एरे में निर्दिष्ट एरे इंडेक्स से शुरू करके कॉपी करता है"
type: docs
weight: 70
url: /hi/net/aspose.tasks/viewcollection/copyto/
---
## ViewCollection.CopyTo method

निर्दिष्ट एरे सूचकांक से शुरू करके इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है।

```csharp
public void CopyTo(View[] array, int arrayIndex)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| एरे | View[] | तत्वों को कॉपी करने के लिए निर्दिष्ट एक-आयामी एरे |
| arrayIndex | Int32 | निर्दिष्ट एरे का शून्य-आधारित इंडेक्स जहाँ से कॉपी शुरू होती है। |

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


