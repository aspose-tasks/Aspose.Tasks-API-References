---
title: "Tsk.SubprojectName"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। उप-प्रोजेक्ट का स्रोत स्थान"
type: docs
weight: 1070
url: /hi/net/aspose.tasks/tsk/subprojectname/
---
## Tsk.SubprojectName field

सबप्रोजेक्ट का स्रोत स्थान।

```csharp
public static readonly Key<string, TaskKey> SubprojectName;
```

## उदाहरण

दिखाता है कि उप-प्रोजेक्ट कार्य कैसे बनाएं।

```csharp
var project = new Project(DataDir + "SubProjectTask.mpp");

// कार्य जोड़ें
var task = project.RootTask.Children.Add("Task 1");

// नया उप-प्रोजेक्ट लिंक सेट करना
task.Set(Tsk.SubprojectName, DataDir + "subProject.mpp");

project.Save(OutDir + "CreateSubProjectTask_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


