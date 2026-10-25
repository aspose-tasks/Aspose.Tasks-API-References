---
title: "TaskUsageView.FieldCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskUsageView प्रॉपर्टी। इस TaskUsageView का TaskUsageViewFieldCollection ऑब्जेक्ट प्राप्त करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/taskusageview/fieldcollection/
---
## TaskUsageView.FieldCollection property

इस TaskUsageView का [`TaskUsageViewFieldCollection`](../../taskusageviewfieldcollection/) ऑब्जेक्ट प्राप्त करता है।

```csharp
public TaskUsageViewFieldCollection FieldCollection { get; }
```

## उदाहरण

दिखाता है कि कैसे टास्क उपयोग दृश्य फ़ील्ड पढ़ें।

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### संबंधित देखें

* class [TaskUsageViewFieldCollection](../../taskusageviewfieldcollection/)
* class [TaskUsageView](../)
* namespace [Aspose.Tasks](../../taskusageview/)
* assembly [Aspose.Tasks](../../../)


