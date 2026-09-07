---
title: "क्लास PrimaveraSaveOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Saving.PrimaveraSaveOptions क्लास. प्रोजेक्ट को Primavera XER फॉर्मेट में सेव करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है"
type: docs
weight: 2150
url: /hi/net/aspose.tasks.saving/primaverasaveoptions/
---
## PrimaveraSaveOptions class

Primavera XER फ़ॉर्मेट में प्रोजेक्ट सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।

```csharp
public class PrimaveraSaveOptions : SimpleSaveOptions
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PrimaveraSaveOptions](primaverasaveoptions/)() | `PrimaveraSaveOptions` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [ActivityIdIncrement](../../aspose.tasks.saving/primaverasaveoptions/activityidincrement/) { get; set; } | एक्टिविटी IDs को री-नंबर करने में उपयोग होने वाले इन्क्रिमेंट को प्राप्त करता है या सेट करता है। |
| [ActivityIdPrefix](../../aspose.tasks.saving/primaverasaveoptions/activityidprefix/) { get; set; } | एक्टिविटी IDs को री-नंबर करने में उपयोग होने वाले प्रीफ़िक्स को प्राप्त करता है या सेट करता है। |
| [ActivityIdSuffix](../../aspose.tasks.saving/primaverasaveoptions/activityidsuffix/) { get; set; } | एक्टिविटी IDs को री-नंबर करने में उपयोग होने वाले सफ़िक्स को प्राप्त करता है या सेट करता है। |
| [RenumberActivityIds](../../aspose.tasks.saving/primaverasaveoptions/renumberactivityids/) { get; set; } | एक्टिविटी IDs को री-नंबर करने की आवश्यकता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | यदि इस सहेजने विकल्प वस्तु का उपयोग किया जाता है तो दस्तावेज़ को सहेजने के लिए उपयोग किए जाने वाले स्वरूप को प्राप्त करता है या सेट करता है। |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि निर्यात के दौरान संसाधनों को समरी टास्क्स को असाइन करना छोड़ दिया जाए या नहीं। |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gantt चार्ट और टास्क शीट चार्ट पर कार्यों को क्रमबद्ध करने के लिए तुलना करने वाले को प्राप्त करता है या सेट करता है। |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gantt, टास्क शीट और टास्क उपयोग चार्ट पर रेंडर किए गए कार्यों को फ़िल्टर करने के लिए उपयोग की जाने वाली शर्त को प्राप्त करता है या सेट करता है। |

## उदाहरण

दिखाता है कि &lt;see cref="Aspose.Tasks.Saving.PrimaveraSaveOptions" /&gt; के साथ कैसे काम किया जाए।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Primavera सेव विकल्प बनाएं और उन्हें ट्यून करें
var options = new PrimaveraSaveOptions
                  {
                      // एक एक्टिविटी का प्रीफ़िक्स और सफ़िक्स परिभाषित करें
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // एक्टिविटीज़ के री-नंबरिंग को नियंत्रित करें
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### संबंधित देखें

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


