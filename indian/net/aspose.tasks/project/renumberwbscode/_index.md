---
title: "Project.RenumberWBSCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project विधि। सभी कार्यों के WBS कोड को पुनः क्रमांकित करता है"
type: docs
weight: 1180
url: /hi/net/aspose.tasks/project/renumberwbscode/
---
## RenumberWBSCode() {#renumberwbscode}

सभी कार्यों के WBS कोड को पुनः क्रमांकित करता है।

```csharp
public void RenumberWBSCode()
```

## उदाहरण

कार्य के WBS कोड को पुनः क्रमांकित करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

IEnumerable<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// आउटपुट: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode();

Console.WriteLine("\nWBS codes after: ");

// आउटपुट: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## RenumberWBSCode(List&lt;int&gt;) {#renumberwbscode_1}

पारित कार्यों के WBS कोड को पुनः क्रमांकित करता है।

```csharp
public void RenumberWBSCode(List<int> taskIds)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| taskIds | List`1 | WBS कोड को पुनः क्रमांकित करने के लिए कार्य पहचानकर्ता। |

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

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


