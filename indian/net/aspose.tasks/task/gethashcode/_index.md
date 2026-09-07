---
title: "Task.GetHashCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task मेथड. इस Task के लिए एक हैश कोड मान लौटाता है"
type: docs
weight: 1350
url: /hi/net/aspose.tasks/task/gethashcode/
---
## Task.GetHashCode method

इस Task के लिए हैश कोड मान लौटाता है।

```csharp
public override int GetHashCode()
```

### रिटर्न वैल्यू

इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।

## उदाहरण

दिखाता है कि टास्क का हैश कोड कैसे प्राप्त किया जाए।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

// एक कार्य का हैश कोड कार्य के UID और नाम पर आधारित होता है
Console.WriteLine("Hash code of the task: " + task.GetHashCode());

task.Set(Tsk.Name, "Task 1");

Console.WriteLine("Hash code of the task: " + task.GetHashCode());
```

### संबंधित देखें

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


