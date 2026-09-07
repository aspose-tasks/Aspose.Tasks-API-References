---
title: "ResourceUsageViewFieldCollection.ToList"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceUsageViewFieldCollection मेथड। ResourceUsageViewFieldCollection क्लास की इंस्टेंस को एक सूची में बदलता है जिसमें ResourceUsageViewField क्लास की इंस्टेंसें शामिल होती हैं"
type: docs
weight: 20
url: /hi/net/aspose.tasks/resourceusageviewfieldcollection/tolist/
---
## ResourceUsageViewFieldCollection.ToList method

[`ResourceUsageViewFieldCollection`](../) क्लास की इंस्टेंस को एक सूची में बदलता है जिसमें [`ResourceUsageViewField`](../../resourceusageviewfield/) क्लास की इंस्टेंसें शामिल होती हैं।

```csharp
public IList<ResourceUsageViewField> ToList()
```

### रिटर्न वैल्यू

[`ResourceUsageViewFieldCollection`](../) क्लास की इंस्टेंस को सूची में बदला गया है जिसमें [`ResourceUsageViewField`](../../resourceusageviewfield/) क्लास की इंस्टेंसें शामिल हैं।

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

* enum [ResourceUsageViewField](../../resourceusageviewfield/)
* class [ResourceUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../resourceusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


