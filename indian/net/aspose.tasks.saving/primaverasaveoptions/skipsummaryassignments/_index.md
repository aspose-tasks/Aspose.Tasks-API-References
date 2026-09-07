---
title: "PrimaveraSaveOptions.SkipSummaryAssignments"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrimaveraSaveOptions प्रॉपर्टी। यह दर्शाने वाला मान प्राप्त करता है या सेट करता है कि निर्यात के दौरान सारांश कार्यों को संसाधनों के असाइनमेंट को छोड़ना चाहिए या नहीं"
type: docs
weight: 60
url: /hi/net/aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/
---
## PrimaveraSaveOptions.SkipSummaryAssignments property

एक मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि निर्यात के दौरान संसाधनों को समरी टास्क्स को असाइन करना छोड़ दिया जाए या नहीं।

```csharp
public bool SkipSummaryAssignments { get; set; }
```

## टिप्पणियाँ

Primavera सॉफ़्टवेयर संसाधनों को सारांश (WBS) टास्कों को असाइन करने का समर्थन नहीं करता है। इसलिए, ऐसे असाइनमेंट का निर्यात Primavera मॉडल के अनुसार एक अमान्य फ़ाइल का परिणाम दे सकता है। यदि true है, तो निर्यात के दौरान सारांश टास्कों को असाइनमेंट छोड़ दिए जाते हैं। यदि false (डिफ़ॉल्ट मान) है, तो निर्यात के दौरान यदि किसी सारांश टास्क को असाइनमेंट मिलता है तो एक अपवाद फेंका जाएगा।

## उदाहरण

दिखाता है कि SkipSummaryAssignments फ़्लैग का उपयोग कैसे करें।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var resource = project.Resources.Add("Resource");

var summaryTask = project.RootTask.Children.Add("Summary");
summaryTask.Children.Add("Task");

// Primavera संसाधनों को सारांश टास्कों को असाइन करने का समर्थन नहीं करता है।
// इसलिए ऐसे असाइनमेंट को Primavera फ़ॉर्मेट में निर्यात करने से ऐसी फ़ाइलें बन सकती हैं जिन्हें Primavera में आयात नहीं किया जा सकता।
var assignment = project.ResourceAssignments.Add(summaryTask, resource);

var options = new PrimaveraXmlSaveOptions();
options.SkipSummaryAssignments = true;
project.Save(OutDir + "UseSkipSummaryAssignments_out.xml", options);
```

### संबंधित देखें

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


