---
title: "CsvOptions.View"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CsvOptions प्रॉपर्टी। व्यू कॉलम GanttChartColumn की सूची प्राप्त करता है या सेट करता है जिसे XLSX फ़ॉर्मेट में सहेजा जाता है। यदि सेट नहीं किया गया तो डिफ़ॉल्ट कॉलम सहेजे जाते हैं"
type: docs
weight: 60
url: /hi/net/aspose.tasks.saving/csvoptions/view/
---
## CsvOptions.View property

व्यू कॉलम की सूची प्राप्त करता है या सेट करता है ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)) जिसे XLSX फ़ॉर्मेट में सहेजा जाता है। यदि सेट नहीं किया गया तो डिफ़ॉल्ट कॉलम सहेजे जाते हैं।

```csharp
public ProjectView View { get; set; }
```

## उदाहरण

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

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


