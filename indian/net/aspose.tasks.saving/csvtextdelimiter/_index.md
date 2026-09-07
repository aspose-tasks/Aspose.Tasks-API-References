---
title: "Enum CsvTextDelimiter"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Saving.CsvTextDelimiter enum. CSV फ़ॉर्मेट के लिए टेक्स्ट डिलिमिटर"
type: docs
weight: 1990
url: /hi/net/aspose.tasks.saving/csvtextdelimiter/
---
## CsvTextDelimiter enumeration

CSV फ़ॉर्मेट के लिए टेक्स्ट डिलिमिटर।

```csharp
public enum CsvTextDelimiter
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Comma | `0` | कॉमा डिलिमिटर। |
| Semicolon | `1` | सेमिकॉलन डिलिमिटर। |
| Space | `2` | स्पेस डिलिमिटर। |
| Tab | `3` | टैब डिलिमिटर। |

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


