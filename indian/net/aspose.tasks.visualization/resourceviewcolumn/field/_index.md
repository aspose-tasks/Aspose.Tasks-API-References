---
title: "ResourceViewColumn.Field"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceViewColumn प्रॉपर्टी। कॉलम फ़ील्ड। फ़ील्ड"
type: docs
weight: 20
url: /hi/net/aspose.tasks.visualization/resourceviewcolumn/field/
---
## ResourceViewColumn.Field property

कॉलम फ़ील्ड। `Field`।

```csharp
public override Field Field { get; set; }
```

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

* enum [Field](../../../aspose.tasks/field/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)


