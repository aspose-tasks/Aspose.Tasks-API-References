---
title: "क्लास XlsxOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Saving.XlsxOptions क्लास। प्रोजेक्ट पेजों को XLSX में रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 2270
url: /hi/net/aspose.tasks.saving/xlsxoptions/
---
## XlsxOptions class

XLSX में प्रोजेक्ट पेज रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।

```csharp
public class XlsxOptions : SimpleSaveOptions
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [XlsxOptions](xlsxoptions/)() | `XlsxOptions` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है जिसे प्रोजेक्ट को XLSX प्रारूप में सहेजने के लिए उपयोग किया जा सकता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/xlsxoptions/assignmentview/) { get; set; } | रेंडर करने के लिए असाइनमेंट व्यू कॉलम की सूची प्राप्त करता है या सेट करता है ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [Encoding](../../aspose.tasks.saving/xlsxoptions/encoding/) { get; set; } | परिणामी XLSX फ़ाइल की एन्कोडिंग को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान UTF8 है। |
| [ResourceView](../../aspose.tasks.saving/xlsxoptions/resourceview/) { get; set; } | रेंडर करने के लिए रिसोर्स व्यू कॉलम की सूची प्राप्त करता है या सेट करता है ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | यदि इस सहेजने विकल्प वस्तु का उपयोग किया जाता है तो दस्तावेज़ को सहेजने के लिए उपयोग किए जाने वाले स्वरूप को प्राप्त करता है या सेट करता है। |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gantt चार्ट और टास्क शीट चार्ट पर कार्यों को क्रमबद्ध करने के लिए तुलना करने वाले को प्राप्त करता है या सेट करता है। |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gantt, टास्क शीट और टास्क उपयोग चार्ट पर रेंडर किए गए कार्यों को फ़िल्टर करने के लिए उपयोग की जाने वाली शर्त को प्राप्त करता है या सेट करता है। |
| [View](../../aspose.tasks.saving/xlsxoptions/view/) { get; set; } | XLSX प्रारूप में सहेजने के लिए दृश्य कॉलमों की सूची ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) को प्राप्त करता है या सेट करता है। यदि सेट नहीं किया गया तो डिफ़ॉल्ट कॉलम सहेजे जाते हैं। |

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


