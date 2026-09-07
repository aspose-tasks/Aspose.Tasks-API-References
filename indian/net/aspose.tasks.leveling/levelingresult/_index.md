---
title: "क्लास LevelingResult"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Leveling.LevelingResult क्लास. रिसोर्स लेवलिंग के परिणामों का प्रतिनिधित्व करता है"
type: docs
weight: 960
url: /hi/net/aspose.tasks.leveling/levelingresult/
---
## LevelingResult class

रिसोर्स लेवलिंग के परिणामों को दर्शाता है।

```csharp
public sealed class LevelingResult
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [LevelingResult](levelingresult/)() | `LevelingResult` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [AffectedTasks](../../aspose.tasks.leveling/levelingresult/affectedtasks/) { get; } | रिसोर्स लेवलिंग से प्रभावित टास्क का सेट प्राप्त करता है। |

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

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


