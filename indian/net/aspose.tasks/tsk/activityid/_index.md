---
title: "Tsk.ActivityId"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। Primavera द्वारा उपयोग किया गया कार्य का अद्वितीय पहचानकर्ता दर्शाता है। केवल Primavera प्रोजेक्ट्स पर लागू।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/tsk/activityid/
---
## Tsk.ActivityId field

गतिविधि आईडी फ़ील्ड का प्रतिनिधित्व करता है - Primavera द्वारा उपयोग किया जाने वाला टास्क का अद्वितीय पहचानकर्ता। (केवल Primavera प्रोजेक्ट्स पर लागू)।

```csharp
public static readonly Key<string, TaskKey> ActivityId;
```

## उदाहरण

दिखाता है कि Primavera प्रोजेक्ट्स के लिए विशिष्ट ActivityId फ़ील्ड के साथ कैसे काम करें

```csharp
var project = new Project(DataDir + "test.xer");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Task activity_id: {0}", task.Get(Tsk.ActivityId));

task.Set(Tsk.ActivityId, "CUSTOM_ACTIVITY_ID");

// Primavera सहेजने विकल्प बनाएं और निर्दिष्ट करें कि सहेजते समय ActivityIds को अधिलेखित नहीं किया जाना चाहिए।
var options = new PrimaveraSaveOptions
{
    RenumberActivityIds = false
};

project.Save(OutDir + "WorkWithPrimaveraActivityId_out.xer", options);
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


