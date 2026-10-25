---
title: "क्लास ViewCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ViewCollection क्लास। View ऑब्जेक्ट्स की सूची रखती है। ICollectionView इंटरफ़ेस को लागू करती है।"
type: docs
weight: 2900
url: /hi/net/aspose.tasks/viewcollection/
---
## ViewCollection class

[`View`](../view/) ऑब्जेक्ट्स की सूची रखती है। ICollection&lt;View&gt; इंटरफ़ेस को लागू करती है।

```csharp
public class ViewCollection : ICollection<View>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/viewcollection/count/) { get; } | इस संग्रह में मौजूद तत्वों की संख्या प्राप्त करता है। |
| [IsReadOnly](../../aspose.tasks/viewcollection/isreadonly/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-रीड है या नहीं; अन्यथा, false। |
| [ParentProject](../../aspose.tasks/viewcollection/parentproject/) { get; } | View ऑब्जेक्ट का पैरेंट प्राप्त करता है। केवल‑पढ़ने योग्य [`Project`](../project/). |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/viewcollection/add/)(View) | निर्दिष्ट आइटम को इस संग्रह में जोड़ता है। |
| [Clear](../../aspose.tasks/viewcollection/clear/)() | इस संग्रह से सभी आइटम हटाता है। |
| [Contains](../../aspose.tasks/viewcollection/contains/)(View) | यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false। |
| [CopyTo](../../aspose.tasks/viewcollection/copyto/)(View[], int) | निर्दिष्ट एरे सूचकांक से शुरू करके इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है। |
| [GetByName](../../aspose.tasks/viewcollection/getbyname/)(string) | नाम के साथ एक View खोजती है, और संग्रह में पहली घटना लौटाती है। |
| [GetByViewScreen](../../aspose.tasks/viewcollection/getbyviewscreen/)(ViewScreen) | निर्दिष्ट Screen प्रॉपर्टी वाले View को खोजती है, और संग्रह में पहली घटना लौटाती है। |
| [GetEnumerator](../../aspose.tasks/viewcollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks/viewcollection/remove/)(View) | इस संग्रह से विशिष्ट वस्तु की पहली घटना को हटाता है। |
| [ToList](../../aspose.tasks/viewcollection/tolist/)() | एक view संग्रह को [`View`](../view/) ऑब्जेक्ट्स की सूची में बदलती है। |

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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


