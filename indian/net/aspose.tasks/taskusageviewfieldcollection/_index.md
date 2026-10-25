---
title: "क्लास TaskUsageViewFieldCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TaskUsageViewFieldCollection क्लास। TaskUsageViewField मानों का संग्रह दर्शाता है।"
type: docs
weight: 2500
url: /hi/net/aspose.tasks/taskusageviewfieldcollection/
---
## TaskUsageViewFieldCollection class

[`TaskUsageViewField`](../taskusageviewfield/) मानों का संग्रह दर्शाता है।

```csharp
public class TaskUsageViewFieldCollection : IList<TaskUsageViewField>
```

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/taskusageviewfieldcollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [ToList](../../aspose.tasks/taskusageviewfieldcollection/tolist/)() | इस संग्रह से सभी आइटम्स को शामिल करने वाली सूची लौटाता है। |

## उदाहरण

TaskUsageView इंस्टेंस के फ़ील्ड संग्रह के साथ कैसे काम करें, यह दर्शाता है।

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// किसी भी व्यक्ति द्वारा संग्रह को TaskUsageViewField की सूची में परिवर्तित किया जा सकता है।
IList<TaskUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### संबंधित देखें

* enum [TaskUsageViewField](../taskusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


