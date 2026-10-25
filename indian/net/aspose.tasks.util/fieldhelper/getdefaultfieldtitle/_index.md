---
title: "FieldHelper.GetDefaultFieldTitle"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "FieldHelper मेथड। विशिष्ट फ़ील्ड का डिफ़ॉल्ट शीर्षक लौटाता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.util/fieldhelper/getdefaultfieldtitle/
---
## FieldHelper.GetDefaultFieldTitle method

विशिष्ट फ़ील्ड का डिफ़ॉल्ट शीर्षक लौटाता है।

```csharp
public static string GetDefaultFieldTitle(Field field)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| फ़ील्ड | फ़ील्ड | डिफ़ॉल्ट शीर्षक प्राप्त करने के लिए फ़ील्ड। |

### रिटर्न वैल्यू

यदि फ़ील्ड को MS Project के दृश्य में प्रदर्शित किया जा सकता है तो विशिष्ट फ़ील्ड का डिफ़ॉल्ट शीर्षक, अन्यथा null।

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

* enum [Field](../../../aspose.tasks/field/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


