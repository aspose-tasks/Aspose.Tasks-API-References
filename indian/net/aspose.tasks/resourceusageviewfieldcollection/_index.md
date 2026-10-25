---
title: "Class ResourceUsageViewFieldCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ResourceUsageViewFieldCollection class. ResourceUsageViewField मानों का एक संग्रह दर्शाता है।"
type: docs
weight: 1830
url: /hi/net/aspose.tasks/resourceusageviewfieldcollection/
---
## ResourceUsageViewFieldCollection class

`ResourceUsageViewField` मानों का एक संग्रह दर्शाता है।

```csharp
public class ResourceUsageViewFieldCollection : IList<ResourceUsageViewField>
```

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/resourceusageviewfieldcollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [ToList](../../aspose.tasks/resourceusageviewfieldcollection/tolist/)() | `ResourceUsageViewFieldCollection` क्लास की इंस्टेंस को एक सूची में परिवर्तित करता है जिसमें [`ResourceUsageViewField`](../resourceusageviewfield/) क्लास की इंस्टेंस शामिल हैं। |

## उदाहरण

ResourceUsageView इंस्टेंस के फ़ील्ड संग्रह के साथ कैसे काम किया जाए, यह दिखाता है।

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// किसी संग्रह को ResourceUsageViewField की सूची में परिवर्तित किया जा सकता है।
IList<ResourceUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### संबंधित देखें

* enum [ResourceUsageViewField](../resourceusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


