---
title: "TaskUsageViewFieldCollection.ToList"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskUsageViewFieldCollection मेथड। इस कलेक्शन की सभी आइटम्स को शामिल करने वाली एक सूची लौटाता है"
type: docs
weight: 20
url: /hi/net/aspose.tasks/taskusageviewfieldcollection/tolist/
---
## TaskUsageViewFieldCollection.ToList method

इस संग्रह से सभी आइटम्स को शामिल करने वाली सूची लौटाता है।

```csharp
public IList<TaskUsageViewField> ToList()
```

### रिटर्न वैल्यू

इस कलेक्शन की सभी आइटम्स को शामिल करने वाली एक सूची लौटाता है।

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

* enum [TaskUsageViewField](../../taskusageviewfield/)
* class [TaskUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../taskusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


