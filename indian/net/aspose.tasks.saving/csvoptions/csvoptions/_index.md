---
title: "CsvOptions.CsvOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CsvOptions कंस्ट्रक्टर। एक नया CsvOptions क्लास का इंस्टेंस इनिशियलाइज़ करता है जिसका उपयोग प्रोजेक्ट को CSV फ़ॉर्मेट में सहेजने के लिए किया जा सकता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.saving/csvoptions/csvoptions/
---
## CsvOptions constructor

एक नया [`CsvOptions`](../) क्लास का इंस्टेंस इनिशियलाइज़ करता है जिसका उपयोग प्रोजेक्ट को CSV फ़ॉर्मेट में सहेजने के लिए किया जा सकता है।

```csharp
public CsvOptions()
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


