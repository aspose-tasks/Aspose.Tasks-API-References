---
title: "Enum ResourceType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ResourceType enum. संसाधन के प्रकार को निर्दिष्ट करता है"
type: docs
weight: 1800
url: /hi/net/aspose.tasks/resourcetype/
---
## ResourceType enumeration

संसाधन के प्रकार को निर्दिष्ट करता है।

```csharp
public enum ResourceType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Material | `0` | सामग्री संसाधन प्रकार को दर्शाता है। |
| Work | `1` | कार्य संसाधन प्रकार को दर्शाता है। |
| Cost | `2` | लागत संसाधन प्रकार को दर्शाता है। |

## उदाहरण

संसाधन प्रकारों के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project();

// एक कार्य संसाधन जोड़ें
var work = project.Resources.Add("Work resource");
work.Set(Rsc.Type, ResourceType.Work);

// एक सामग्री संसाधन जोड़ें
var material = project.Resources.Add("Material resource");
material.Set(Rsc.Type, ResourceType.Material);
material.Set(Rsc.MaterialLabel, "kg");

// एक सामग्री संसाधन जोड़ें
var cost = project.Resources.Add("Cost resource");
cost.Set(Rsc.Type, ResourceType.Cost);
cost.Set(Rsc.Cost, 59.99m);

// संसाधनों के साथ काम करें: कार्य बनाएं, संसाधन असाइन करें आदि...
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


