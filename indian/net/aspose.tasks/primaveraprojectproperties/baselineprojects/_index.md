---
title: "PrimaveraProjectProperties.BaselineProjects"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrimaveraProjectProperties प्रॉपर्टी। वर्तमान प्रोजेक्ट के बेसलाइन प्रोजेक्ट्स की एरे प्राप्त करता है। यह उन प्रोजेक्ट्स पर लागू होता है जो निर्यातित बेसलाइन वाले Primavera XML फ़ाइलों से पढ़े गए हैं।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/primaveraprojectproperties/baselineprojects/
---
## PrimaveraProjectProperties.BaselineProjects property

वर्तमान प्रोजेक्ट के बेसलाइन प्रोजेक्ट्स की एरे प्राप्त करता है। यह उन प्रोजेक्ट्स पर लागू होता है जो निर्यातित बेसलाइन वाली Primavera XML फ़ाइलों से पढ़े गए हैं।

```csharp
public Project[] BaselineProjects { get; }
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

* class [Project](../../project/)
* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


