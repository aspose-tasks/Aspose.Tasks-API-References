---
title: "ResourceUsageView.FieldCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceUsageView प्रॉपर्टी। इस ResourceUsageView का ResourceUsageViewFieldCollection ऑब्जेक्ट प्राप्त करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/resourceusageview/fieldcollection/
---
## ResourceUsageView.FieldCollection property

इस ResourceUsageView का [`ResourceUsageViewFieldCollection`](../../resourceusageviewfieldcollection/) ऑब्जेक्ट प्राप्त करता है।

```csharp
public ResourceUsageViewFieldCollection FieldCollection { get; }
```

## उदाहरण

संसाधन उपयोग दृश्य फ़ील्ड को कैसे पढ़ें, यह दिखाता है।

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### संबंधित देखें

* class [ResourceUsageViewFieldCollection](../../resourceusageviewfieldcollection/)
* class [ResourceUsageView](../)
* namespace [Aspose.Tasks](../../resourceusageview/)
* assembly [Aspose.Tasks](../../../)


