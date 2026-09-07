---
title: "Enum RateScaleType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.RateScaleType enum। दर स्केल प्रकार को निर्दिष्ट करता है।"
type: docs
weight: 1650
url: /hi/net/aspose.tasks/ratescaletype/
---
## RateScaleType enumeration

दर स्केल प्रकार को निर्दिष्ट करता है।

```csharp
public enum RateScaleType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `0` | Undefined दर स्केल प्रकार को दर्शाता है। |
| Minute | `1` | Minute दर स्केल प्रकार को दर्शाता है। |
| Hour | `2` | Hour दर स्केल प्रकार को दर्शाता है। |
| Day | `3` | Day दर स्केल प्रकार को दर्शाता है। |
| Week | `4` | Week दर स्केल प्रकार को दर्शाता है। |
| Month | `5` | Month दर स्केल प्रकार को दर्शाता है। |
| Quarter | `6` | Quarter दर स्केल प्रकार को दर्शाता है। |
| Year | `7` | Year दर स्केल प्रकार को दर्शाता है। |

## उदाहरण

एक सामग्री संसाधन के असाइनमेंट के लिए परिवर्ती सामग्री खपत (जैसे '10/day' या '1/week') सेट करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// मान लीजिए हम '1/week' सामग्री खपत सेट करना चाहते हैं।
materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);
```

जब हम सामग्री संसाधन के असाइनमेंट के लिए परिवर्ती सामग्री खपत (जैसे '10/day' या '1/week') सेट करना चाहते हैं, तब असाइनमेंट के दर स्केल के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var nonMaterialResource = project.Resources.Add("nonMaterialResource");
nonMaterialResource.Set(Rsc.Type, ResourceType.Work);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// मान लीजिए हम '1/week' सामग्री खपत सेट करना चाहते हैं।
// हमें Units प्रॉपर्टी में घंटे की दर सेट करनी चाहिए, इसलिए हम 1D को सप्ताह के घंटों से विभाजित करते हैं।
materialResourceAssignment.Set(Asn.Units, 1D / 40);
materialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

// कृपया ध्यान दें कि संस्करण 24.4 से यह एक मेथड को कॉल करके किया जा सकता है:
// materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);

var nonMaterialResourceAssignment = project.ResourceAssignments.Add(task, nonMaterialResource);
nonMaterialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

project.Save(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp", SaveFileFormat.Mpp);

var resavedProject = new Project(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp");

var resavedMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(2);
Console.WriteLine(resavedMaterialResourceAssignment.Get(Asn.RateScale));

// केवल सामग्री संसाधन असाइनमेंट में गैर-शून्य दर स्केल मान हो सकता है।
var resavedNonMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(3);
Console.WriteLine(resavedNonMaterialResourceAssignment.Get(Asn.RateScale));
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


