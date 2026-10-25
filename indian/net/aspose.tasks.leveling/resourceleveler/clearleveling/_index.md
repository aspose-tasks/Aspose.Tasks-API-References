---
title: "ResourceLeveler.ClearLeveling"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceLeveler मेथड। रिसोर्स लेवलिंग के दौरान प्रोजेक्ट में पहले जोड़ी गई किसी भी लेवलिंग डिले को साफ़ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.leveling/resourceleveler/clearleveling/
---
## ClearLeveling(Project) {#clearleveling}

संसाधन लेवलिंग के दौरान प्रोजेक्ट में पहले जोड़ी गई किसी भी लेवलिंग देरी को साफ़ करता है।

```csharp
public static void ClearLeveling(Project project)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रोजेक्ट | Project | लेवलिंग को साफ़ करने के लिए प्रोजेक्ट। |

## उदाहरण

डिफ़ॉल्ट विकल्पों का उपयोग करके सभी प्रोजेक्ट संसाधनों को लेवल करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingResult = ResourceLeveler.LevelAll(project);

foreach (var task in levelingResult.AffectedTasks)
{
    Console.WriteLine("Task affected by the leveling operation: " + task.Name);
}

project.Save(OutDir + "Software Development Plan.leveled.mpp");
ResourceLeveler.ClearLeveling(project);

Console.WriteLine("Leveling cleared");
```

### संबंधित देखें

* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)

---

## ClearLeveling(IEnumerable&lt;Task&gt;) {#clearleveling_1}

संसाधन लेवलिंग के दौरान निर्दिष्ट कार्यों में पहले जोड़ी गई किसी भी लेवलिंग देरी को साफ़ करता है।

```csharp
public static void ClearLeveling(IEnumerable<Task> tasks)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कार्य | IEnumerable`1 | इटेरेबल जिसमें उन कार्यों को शामिल किया गया है जिनके लिए लेवलिंग डिले को साफ़ किया जाना चाहिए। |

### संबंधित देखें

* class [Task](../../../aspose.tasks/task/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


