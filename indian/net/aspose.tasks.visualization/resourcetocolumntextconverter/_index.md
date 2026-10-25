---
title: "डेलीगेट ResourceToColumnTextConverter"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "संसाधनों का डेटा कॉलम स्ट्रिंग कनवर्टर"
type: docs
weight: 3340
url: /hi/net/aspose.tasks.visualization/resourcetocolumntextconverter/
---
## ResourceToColumnTextConverter delegate

संसाधन डेटा को कॉलम की स्ट्रिंग में बदलने वाला कनवर्टर।

```csharp
public delegate string ResourceToColumnTextConverter(Resource resource);
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| संसाधन | संसाधन | वर्तमान संसाधन। |

### रिटर्न वैल्यू

कॉलम के लिए स्ट्रिंग डेटा।

## उदाहरण

निर्यात के लिए संसाधन व्यू कॉलम कैसे जोड़ें, यह दिखाता है।

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);

var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new ResourceViewColumn(100, Field.ResourceName),
    new ResourceViewColumn(100, Field.ResourceActualWork),
    new ResourceViewColumn(100, Field.ResourceCost),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }, 
        Field.ResourceCost2)
};

// कॉलम पर इटररेट करें
foreach (var column in columns)
{
    var col = (ResourceViewColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(resource));
    Console.WriteLine();
}

options.View = new ProjectView(columns);
options.PresentationFormat = PresentationFormat.ResourceUsage;
project.Save(OutDir + "WorkWithAssignmentViewColumn_out.pdf", options);
```

### संबंधित देखें

* class [Resource](../../aspose.tasks/resource/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


