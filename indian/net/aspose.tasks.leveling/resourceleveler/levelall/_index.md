---
title: "ResourceLeveler.LevelAll"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceLeveler मेथड। डिफ़ॉल्ट लेवलिंग विकल्पों का उपयोग करके सभी प्रोजेक्ट्स के संसाधनों के लिए कार्यों को लेवल करता है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.leveling/resourceleveler/levelall/
---
## ResourceLeveler.LevelAll method

डिफ़ॉल्ट लेवलिंग विकल्पों का उपयोग करके सभी प्रोजेक्ट संसाधनों के लिए कार्यों को लेवल करता है।

```csharp
public static LevelingResult LevelAll(Project project)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रोजेक्ट | Project | रिसोर्स लेवलिंग लागू करने के लिए प्रोजेक्ट। |

### रिटर्न वैल्यू

ऑब्जेक्ट जिसमें रिसोर्स लेवलिंग के परिणाम होते हैं।

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


