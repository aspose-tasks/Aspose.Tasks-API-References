---
title: "क्लास PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Saving.PrimaveraXmlSaveOptions क्लास। प्रोजेक्ट को Primavera XML फ़ॉर्मेट में सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है"
type: docs
weight: 2160
url: /hi/net/aspose.tasks.saving/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions class

Primavera XML फ़ॉर्मेट में प्रोजेक्ट सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।

```csharp
public class PrimaveraXmlSaveOptions : SimpleSaveOptions
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PrimaveraXmlSaveOptions](primaveraxmlsaveoptions/)() | `PrimaveraXmlSaveOptions` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | यदि इस सहेजने विकल्प वस्तु का उपयोग किया जाता है तो दस्तावेज़ को सहेजने के लिए उपयोग किए जाने वाले स्वरूप को प्राप्त करता है या सेट करता है। |
| [SaveRootTask](../../aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि रूट टास्क को सहेजा जाए या नहीं। |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि निर्यात के दौरान संसाधनों को समरी टास्क्स को असाइन करना छोड़ दिया जाए या नहीं। |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gantt चार्ट और टास्क शीट चार्ट पर कार्यों को क्रमबद्ध करने के लिए तुलना करने वाले को प्राप्त करता है या सेट करता है। |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gantt, टास्क शीट और टास्क उपयोग चार्ट पर रेंडर किए गए कार्यों को फ़िल्टर करने के लिए उपयोग की जाने वाली शर्त को प्राप्त करता है या सेट करता है। |

## उदाहरण

दिखाता है कि Primavera XML फ़ाइल में कैसे निर्यात किया जाए।

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### संबंधित देखें

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


