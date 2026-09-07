---
title: "ResourceUsageViewFieldCollection.GetEnumerator"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceUsageViewFieldCollection मेथड। इस संग्रह के लिए एक एनेमरेटर लौटाता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/resourceusageviewfieldcollection/getenumerator/
---
## ResourceUsageViewFieldCollection.GetEnumerator method

इस संग्रह के लिए एक एन्यूमरेटर लौटाता है।

```csharp
public IEnumerator<ResourceUsageViewField> GetEnumerator()
```

### रिटर्न वैल्यू

इस संग्रह के लिए एक एनेमरेटर।

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


