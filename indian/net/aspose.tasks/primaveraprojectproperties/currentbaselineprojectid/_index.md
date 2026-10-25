---
title: "PrimaveraProjectProperties.CurrentBaselineProjectId"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrimaveraProjectProperties प्रॉपर्टी। वर्तमान बेसलाइन प्रोजेक्ट का Id प्राप्त करता है। यह उन प्रोजेक्ट्स पर लागू होता है जो निर्यातित बेसलाइन वाले Primavera XML फ़ाइलों से पढ़े जाते हैं।"
type: docs
weight: 40
url: /hi/net/aspose.tasks/primaveraprojectproperties/currentbaselineprojectid/
---
## PrimaveraProjectProperties.CurrentBaselineProjectId property

वर्तमान बेसलाइन प्रोजेक्ट का Id प्राप्त करता है। यह निर्यातित बेसलाइन वाली Primavera XML फ़ाइलों से पढ़े गए प्रोजेक्ट्स पर लागू होता है।

```csharp
public int CurrentBaselineProjectId { get; }
```

## उदाहरण

दिखाता है कि Primavera XML फ़ाइल से प्रोजेक्ट कैसे पढ़ें और बेसलाइन प्रोजेक्ट डेटा की जांच करें।

```csharp
Project project = new Project(DataDir + "BaselineProjects.xml");

Console.WriteLine("Current baseline project uid: " + project.PrimaveraProperties.CurrentBaselineProjectId);

foreach (var baselineProject in project.PrimaveraProperties.BaselineProjects)
{
    Console.WriteLine("Baseline project: uid: {0}, name: '{1}'", baselineProject.Uid, baselineProject.Name);
}

var baseline1 = project.PrimaveraProperties.BaselineProjects[1];

var task = GetTaskByActivityId(project, "A1000");
var baselineTask = GetTaskByActivityId(baseline1, "A1000");

Console.WriteLine("Task budgeted total cost: " + task.PrimaveraProperties.BudgetedTotalCost);
Console.WriteLine("Task baseline budgeted total cost: " + baselineTask.PrimaveraProperties.BudgetedTotalCost);
```

### संबंधित देखें

* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


