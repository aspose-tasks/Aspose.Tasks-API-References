---
title: "CsvOptions.IncludeHeaders"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CsvOptions प्रॉपर्टी. एक मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि हेडर शामिल करना है या नहीं, डिफ़ॉल्ट मान TRUE है"
type: docs
weight: 40
url: /hi/net/aspose.tasks.saving/csvoptions/includeheaders/
---
## CsvOptions.IncludeHeaders property

हेडर शामिल करना है या नहीं (डिफ़ॉल्ट मान TRUE है) यह दर्शाने वाला मान प्राप्त करता है या सेट करता है।

```csharp
public bool IncludeHeaders { get; set; }
```

## उदाहरण

दिखाता है कि कैसे &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; का उपयोग करके प्रोजेक्ट को CSV फ़ाइल के रूप में सहेजा जाए।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var options = new CsvOptions
{
    DataCategory = DataCategory.Resources,
    TextDelimiter = CsvTextDelimiter.Semicolon,
    Encoding = Encoding.Unicode, IncludeHeaders = true
};

project.Save(OutDir + "WorkWithCsvOptions_out.csv", options);
```

### संबंधित देखें

* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


