---
title: "क्लास CsvOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Saving.CsvOptions क्लास। प्रोजेक्ट को CSV में सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देती है।"
type: docs
weight: 1980
url: /hi/net/aspose.tasks.saving/csvoptions/
---
## CsvOptions class

CSV में प्रोजेक्ट सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।

```csharp
public class CsvOptions : SimpleSaveOptions
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [CsvOptions](csvoptions/)() | `CsvOptions` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है जिसका उपयोग प्रोजेक्ट को CSV फ़ॉर्मेट में सहेजने के लिए किया जा सकता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [DataCategory](../../aspose.tasks.saving/csvoptions/datacategory/) { get; set; } | सहेजे जाने वाले डेटा श्रेणी को प्राप्त करता है या सेट करता है। |
| [Encoding](../../aspose.tasks.saving/csvoptions/encoding/) { get; set; } | CSV को सहेजने के लिए एन्कोडिंग प्राप्त करता है या सेट करता है। |
| [IncludeHeaders](../../aspose.tasks.saving/csvoptions/includeheaders/) { get; set; } | हेडर शामिल करना है या नहीं (डिफ़ॉल्ट मान TRUE है) यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | यदि इस सहेजने विकल्प वस्तु का उपयोग किया जाता है तो दस्तावेज़ को सहेजने के लिए उपयोग किए जाने वाले स्वरूप को प्राप्त करता है या सेट करता है। |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gantt चार्ट और टास्क शीट चार्ट पर कार्यों को क्रमबद्ध करने के लिए तुलना करने वाले को प्राप्त करता है या सेट करता है। |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gantt, टास्क शीट और टास्क उपयोग चार्ट पर रेंडर किए गए कार्यों को फ़िल्टर करने के लिए उपयोग की जाने वाली शर्त को प्राप्त करता है या सेट करता है। |
| [TextDelimiter](../../aspose.tasks.saving/csvoptions/textdelimiter/) { get; set; } | पाठ विभाजक को प्राप्त करता है या सेट करता है। |
| [View](../../aspose.tasks.saving/csvoptions/view/) { get; set; } | XLSX प्रारूप में सहेजने के लिए दृश्य कॉलमों की सूची ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) को प्राप्त करता है या सेट करता है। यदि सेट नहीं किया गया तो डिफ़ॉल्ट कॉलम सहेजे जाते हैं। |

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

डिफ़ॉल्ट गैंट चार्ट के कॉलम लेने के लिए &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; का उपयोग कैसे करें, यह दिखाता है और

```csharp
// उन्हें CSV फ़ाइल में सहेजें।
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

CsvOptions options = new CsvOptions();
options.TextDelimiter = CsvTextDelimiter.Tab;

var view = project.DefaultView;
options.View = ProjectView.GetDefaultGanttChartView();
options.View.Columns.Clear();

foreach (var t in view.Table.TableFields)
{
    var columnTitle = string.IsNullOrEmpty(t.Title) ? FieldHelper.GetDefaultFieldTitle(t.Field) : t.Title;
    options.View.Columns.Add(new GanttChartColumn(columnTitle, 10, t.Field));
}

project.Save(OutDir + "CustomizeViewForCsvOptions_out.csv", options);
```

### संबंधित देखें

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


