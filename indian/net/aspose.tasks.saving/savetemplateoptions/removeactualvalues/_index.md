---
title: "SaveTemplateOptions.RemoveActualValues"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveTemplateOptions प्रॉपर्टी। वह मान प्राप्त करता है या सेट करता है जो दर्शाता है कि प्रोजेक्ट टेम्प्लेट से सभी वास्तविक मान हटाए जाने चाहिए या नहीं।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.saving/savetemplateoptions/removeactualvalues/
---
## SaveTemplateOptions.RemoveActualValues property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि प्रोजेक्ट टेम्प्लेट से सभी वास्तविक मानों को हटाया जाना चाहिए या नहीं।

```csharp
public bool RemoveActualValues { get; set; }
```

## उदाहरण

विकल्पों का उपयोग करके प्रोजेक्ट को टेम्प्लेट के रूप में सहेजना कैसे दिखाता है।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "EstimatedMilestoneTasks.mpp");

Console.WriteLine("Project File Format: " + projectFileInfo.ProjectFileFormat);

// टेम्प्लेट सहेजने के विकल्प बनाएं
// और इसकी प्रॉपर्टीज़ को ट्यून करें
var options = new SaveTemplateOptions
{
    // एक मान सेट करें जो दर्शाता है कि प्रोजेक्ट टेम्प्लेट से सभी निश्चित लागतों को हटाया जाना चाहिए या नहीं
    RemoveFixedCosts = true,

    // एक मान सेट करें जो दर्शाता है कि प्रोजेक्ट टेम्प्लेट से सभी वास्तविक मानों को हटाया जाना चाहिए या नहीं
    RemoveActualValues = true,

    // एक मान सेट करें जो दर्शाता है कि प्रोजेक्ट टेम्प्लेट से संसाधन दरों को हटाया जाना चाहिए या नहीं
    RemoveResourceRates = true,

    // एक मान सेट करें जो दर्शाता है कि प्रोजेक्ट टेम्प्लेट से सभी बेसलाइन मानों को हटाया जाना चाहिए या नहीं
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(DataDir + "SaveProjectDataAsTemplate_out.mpt");
Console.WriteLine("Project File Format: " + templateFileInfo.ProjectFileFormat);
```

### संबंधित देखें

* class [SaveTemplateOptions](../)
* namespace [Aspose.Tasks.Saving](../../savetemplateoptions/)
* assembly [Aspose.Tasks](../../../)


