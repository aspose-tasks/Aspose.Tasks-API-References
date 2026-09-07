---
title: "ResourceViewColumn.GetColumnText"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceViewColumn मेथड। वर्तमान रिसोर्स को कॉलम टेक्स्ट में बदलता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks.visualization/resourceviewcolumn/getcolumntext/
---
## ResourceViewColumn.GetColumnText method

वर्तमान संसाधन को कॉलम टेक्स्ट में परिवर्तित करता है।

```csharp
public string GetColumnText(Resource resource)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| संसाधन | संसाधन | वर्तमान संसाधन। |

### रिटर्न वैल्यू

कॉलम टेक्स्ट।

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

* class [Resource](../../../aspose.tasks/resource/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)


