---
title: "Enum DataCategory"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Saving.DataCategory enum. CSV में सहेजते समय उपयोग किए जाने वाले डेटा की श्रेणी।"
type: docs
weight: 2000
url: /hi/net/aspose.tasks.saving/datacategory/
---
## DataCategory enumeration

CSV में सहेजते समय उपयोग किए जाने वाले डेटा की श्रेणी।

```csharp
public enum DataCategory
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Tasks | `0` | कार्य जानकारी। |
| Resources | `1` | संसाधन जानकारी। |
| Assignments | `2` | असाइनमेंट जानकारी। |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


