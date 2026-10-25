---
title: "Task.Children"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task प्रॉपर्टी। इस ऑब्जेक्ट का चाइल्ड टास्क कलेक्शन प्राप्त करता है। TaskCollection ऑब्जेक्ट जो चाइल्ड टास्क को दर्शाता है"
type: docs
weight: 190
url: /hi/net/aspose.tasks/task/children/
---
## Task.Children property

इस ऑब्जेक्ट का चाइल्ड टास्क कलेक्शन प्राप्त करता है। TaskCollection ऑब्जेक्ट जो चाइल्ड टास्क को दर्शाता है।

```csharp
public TaskCollection Children { get; }
```

## उदाहरण

दिखाता है कि टास्क कलेक्शन का उपयोग करके टास्क कैसे जोड़ा जाए।

```csharp
var project = new Project();

// टास्क, सब टास्क जोड़ें और प्रोजेक्ट सहेजें
var task = project.RootTask.Children.Add("Summary1");
task.Children.Add("Subtask1");
project.Save(OutDir + "CreateTasks_out.xml", SaveFileFormat.Xml);
```

### संबंधित देखें

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


