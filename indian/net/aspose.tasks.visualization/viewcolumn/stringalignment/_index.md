---
title: "ViewColumn.StringAlignment"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ViewColumn प्रॉपर्टी। टेक्स्ट की अलाइनमेंट प्राप्त करता है या सेट करता है, जो HorizontalStringAlignment एनेमरेशन के मानों में से एक हो सकता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks.visualization/viewcolumn/stringalignment/
---
## ViewColumn.StringAlignment property

टेक्स्ट की अलाइनमेंट प्राप्त करता है या सेट करता है (जो [`HorizontalStringAlignment`](../../horizontalstringalignment/) एनेमरेशन के मानों में से एक हो सकता है)।

```csharp
public HorizontalStringAlignment StringAlignment { get; set; }
```

## उदाहरण

दिखाता है कि कॉलम में टेक्स्ट की संरेखण कैसे सेट करें (यह &lt;see cref="P:Aspose.Tasks.Visualization.ViewColumn.StringAlignment" /&gt; enumeration के मानों में से एक हो सकता है)।

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions();
options.Timescale = Timescale.Months;
options.View = ProjectView.GetDefaultGanttChartView();

var column1 = (GanttChartColumn)options.View.Columns[2];
column1.StringAlignment = HorizontalStringAlignment.Center;
var column2 = (GanttChartColumn)options.View.Columns[3];
column2.StringAlignment = HorizontalStringAlignment.Far;
var column3 = (GanttChartColumn)options.View.Columns[4];
column3.StringAlignment = HorizontalStringAlignment.Far;

project.Save(OutDir + "AlignCellContents_GanttChart_out.pdf", options);

options.PresentationFormat = PresentationFormat.ResourceSheet;
options.View = ProjectView.GetDefaultResourceSheetView();

var column4 = (ResourceViewColumn)options.View.Columns[2];
column4.StringAlignment = HorizontalStringAlignment.Center;
var column5 = (ResourceViewColumn)options.View.Columns[3];
column5.StringAlignment = HorizontalStringAlignment.Far;
var column6 = (ResourceViewColumn)options.View.Columns[4];
column6.StringAlignment = HorizontalStringAlignment.Far;

project.Save(OutDir + "AlignCellContents_ResourceSheet_out.pdf", options);
```

### संबंधित देखें

* enum [HorizontalStringAlignment](../../horizontalstringalignment/)
* class [ViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../viewcolumn/)
* assembly [Aspose.Tasks](../../../)


