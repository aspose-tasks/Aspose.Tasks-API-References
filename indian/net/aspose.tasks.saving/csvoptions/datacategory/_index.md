---
title: "CsvOptions.DataCategory"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CsvOptions प्रॉपर्टी. सहेजे जाने वाले डेटा श्रेणी को प्राप्त करता है या सेट करता है"
type: docs
weight: 20
url: /hi/net/aspose.tasks.saving/csvoptions/datacategory/
---
## CsvOptions.DataCategory property

सहेजे जाने वाले डेटा श्रेणी को प्राप्त करता है या सेट करता है।

```csharp
public DataCategory DataCategory { get; set; }
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

* enum [DataCategory](../../datacategory/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


