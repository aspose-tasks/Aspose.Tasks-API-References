---
title: "Project.SelectAllChildTasks"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project विधि। मूल कार्य की सभी उप-कार्य को पुनरावर्ती रूप से एकत्रित करता है"
type: docs
weight: 1230
url: /hi/net/aspose.tasks/project/selectallchildtasks/
---
## Project.SelectAllChildTasks method

रूट कार्य के सभी चाइल्ड कार्यों को पुनरावर्ती रूप से एकत्र करता है।

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### रिटर्न वैल्यू

कार्य का संग्रह।

## उदाहरण

चयनित कार्यों के WBS कोड को पुनः क्रमांकित करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

var tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// आउटपुट: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode(new List<int> { 1, 2, 3 });

Console.WriteLine("\nWBS codes after: ");

// आउटपुट: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### संबंधित देखें

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


