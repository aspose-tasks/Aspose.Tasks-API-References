---
title: "क्लास SaveTemplateOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Saving.SaveTemplateOptions क्लास. प्रोजेक्ट को टेम्प्लेट के रूप में सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 2200
url: /hi/net/aspose.tasks.saving/savetemplateoptions/
---
## SaveTemplateOptions class

टेम्प्लेट के रूप में प्रोजेक्ट सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।

```csharp
public class SaveTemplateOptions
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [SaveTemplateOptions](savetemplateoptions/)() | डिफ़ॉल्ट कन्स्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [RemoveActualValues](../../aspose.tasks.saving/savetemplateoptions/removeactualvalues/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि प्रोजेक्ट टेम्प्लेट से सभी वास्तविक मानों को हटाया जाना चाहिए या नहीं। |
| [RemoveBaselineValues](../../aspose.tasks.saving/savetemplateoptions/removebaselinevalues/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि प्रोजेक्ट टेम्प्लेट से सभी बेसलाइन मानों को हटाया जाना चाहिए या नहीं। |
| [RemoveFixedCosts](../../aspose.tasks.saving/savetemplateoptions/removefixedcosts/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि प्रोजेक्ट टेम्प्लेट से सभी निश्चित लागतों को हटाया जाना चाहिए या नहीं। |
| [RemoveResourceRates](../../aspose.tasks.saving/savetemplateoptions/removeresourcerates/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि प्रोजेक्ट टेम्प्लेट से संसाधन दरों को हटाया जाना चाहिए या नहीं। |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


