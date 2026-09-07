---
title: "Project.RootTask"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। कार्यों के पेड़ की जड़ प्राप्त करता है"
type: docs
weight: 800
url: /hi/net/aspose.tasks/project/roottask/
---
## Project.RootTask property

कार्य के वृक्ष की मूल प्राप्त करता है।

```csharp
public Task RootTask { get; }
```

## उदाहरण

रूट प्रोजेक्ट टास्क का उपयोग करके प्रोजेक्ट में टास्क जोड़ने का तरीका दिखाता है।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddNewTask_out.xml", SaveFileFormat.Xml);
```

### संबंधित देखें

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


