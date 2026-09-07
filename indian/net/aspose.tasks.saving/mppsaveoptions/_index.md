---
title: "क्लास MPPSaveOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Saving.MPPSaveOptions क्लास। प्रोजेक्ट डेटा को MPP में सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है"
type: docs
weight: 2050
url: /hi/net/aspose.tasks.saving/mppsaveoptions/
---
## MPPSaveOptions class

MPP में प्रोजेक्ट डेटा सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।

```csharp
public class MPPSaveOptions : SimpleSaveOptions
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [MPPSaveOptions](mppsaveoptions/)() | `MPPSaveOptions` क्लास का एक नया उदाहरण आरंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [ClearVba](../../aspose.tasks.saving/mppsaveoptions/clearvba/) { get; set; } | प्रोजेक्ट को MPP फ़ॉर्मेट में सहेजते समय मौजूदा VBA मैक्रो डेटा को हटाने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। |
| [ProtectionPassword](../../aspose.tasks.saving/mppsaveoptions/protectionpassword/) { get; set; } | परिणामी MPP फ़ाइल की सुरक्षा के लिए उपयोग किया जाने वाला पासवर्ड प्राप्त करता है या सेट करता है। वर्तमान में MS Project 2010 और नए फ़ॉर्मेट्स के लिए समर्थित है। शून्य मान दर्शाता है कि प्रोजेक्ट फ़ाइल संरक्षित नहीं है। |
| [RemoveInvalidAssignments](../../aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/) { get; set; } | MPP में सहेजते समय अमान्य संसाधन असाइनमेंट को हटाने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। MS Project प्रत्येक कार्य के लिए एक खाली संसाधन असाइनमेंट बनाता है। सहेजते समय उन्हें हटाने के लिए इस फ़्लैग को true सेट करें। |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | यदि इस सहेजने विकल्प वस्तु का उपयोग किया जाता है तो दस्तावेज़ को सहेजने के लिए उपयोग किए जाने वाले स्वरूप को प्राप्त करता है या सेट करता है। |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gantt चार्ट और टास्क शीट चार्ट पर कार्यों को क्रमबद्ध करने के लिए तुलना करने वाले को प्राप्त करता है या सेट करता है। |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gantt, टास्क शीट और टास्क उपयोग चार्ट पर रेंडर किए गए कार्यों को फ़िल्टर करने के लिए उपयोग की जाने वाली शर्त को प्राप्त करता है या सेट करता है। |
| [WriteFilters](../../aspose.tasks.saving/mppsaveoptions/writefilters/) { get; set; } | प्रोजेक्ट को MPP फ़ॉर्मेट में सहेजते समय फ़िल्टर डेटा लिखने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। फ़िल्टर डेटा में Project.TaskFilters और Project.ResourceFilters संग्रह शामिल हैं। |
| [WriteGroups](../../aspose.tasks.saving/mppsaveoptions/writegroups/) { get; set; } | प्रोजेक्ट को MPP फ़ॉर्मेट में सहेजते समय समूह डेटा लिखने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। समूह डेटा में Project.TaskGroups और Project.ResourceGroups संग्रह शामिल हैं। |
| [WriteVba](../../aspose.tasks.saving/mppsaveoptions/writevba/) { get; set; } | MPP फ़ाइल में मौजूदा VBA मैक्रो डेटा को अपडेट करने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। वर्तमान में VbaModule.SourceCode की लेखन समर्थित है। |
| [WriteViewData](../../aspose.tasks.saving/mppsaveoptions/writeviewdata/) { get; set; } | प्रोजेक्ट को MPP फ़ॉर्मेट में सहेजते समय व्यू डेटा लिखने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। व्यू डेटा में Project.Views, Filters और Tables संग्रह शामिल हैं। |

## उदाहरण

दिखाता है कि प्रोजेक्ट को स्ट्रीम में MPP फ़ाइल के रूप में कैसे सहेजा जाए।

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

    // सेव विकल्प बनाएं
    SimpleSaveOptions options = new MPPSaveOptions
    {
        // MPP में सहेजते समय अमान्य संसाधन असाइनमेंट को हटाने का संकेत देने वाला मान सेट करता है
        RemoveInvalidAssignments = true
    };

    // विकल्पों के साथ MPP सहेजें
    project.Save(stream, options);
}
```

### संबंधित देखें

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


