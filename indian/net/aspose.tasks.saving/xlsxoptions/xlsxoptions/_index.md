---
title: "XlsxOptions.XlsxOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "XlsxOptions कन्स्ट्रक्टर। एक नया इंस्टेंस इनिशियलाइज़ करता है XlsxOptions क्लास का जिसे XLSX फॉर्मेट में प्रोजेक्ट सहेजने के लिए उपयोग किया जा सकता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.saving/xlsxoptions/xlsxoptions/
---
## XlsxOptions constructor

एक नया इंस्टेंस इनिशियलाइज़ करता है [`XlsxOptions`](../) क्लास का जिसे XLSX फॉर्मेट में प्रोजेक्ट सहेजने के लिए उपयोग किया जा सकता है।

```csharp
public XlsxOptions()
```

## उदाहरण

प्रोजेक्ट को XLSX फ़ाइल में सहेजने के लिए &lt;see cref=\"P:Aspose.Tasks.Saving.XlsxOptions\"&gt;Days&lt;/see&gt; विकल्पों का उपयोग कैसे करें, यह दिखाता है।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new XlsxOptions();

// वांछित Gantt Chart कॉलम जोड़ें
var col = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(col);

// वांछित रिसोर्स व्यू कॉलम जोड़ें
var rscCol = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(rscCol);

// वांछित असाइनमेंट व्यू कॉलम जोड़ें
var assnCol = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assnCol);

// एन्कोडिंग सेट करें
options.Encoding = Encoding.Unicode;

project.Save(OutDir + "UsingXlsxOptions_out.xlsx", options);
```

### संबंधित देखें

* class [XlsxOptions](../)
* namespace [Aspose.Tasks.Saving](../../xlsxoptions/)
* assembly [Aspose.Tasks](../../../)


