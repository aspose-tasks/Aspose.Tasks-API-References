---
title: "क्लास ResourceViewColumn"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.ResourceViewColumn क्लास। प्रोजेक्ट्स व्यू क्लास जो ResourceUsage व्यू और ResourceSheet व्यू में उपयोग होती है।"
type: docs
weight: 3350
url: /hi/net/aspose.tasks.visualization/resourceviewcolumn/
---
## ResourceViewColumn class

ResourceUsage दृश्य और ResourceSheet दृश्य में उपयोग किया जाने वाला प्रोजेक्ट का दृश्य वर्ग।

```csharp
public sealed class ResourceViewColumn : ViewColumn
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ResourceViewColumn](resourceviewcolumn/#constructor)(int, Field) | `ResourceViewColumn` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [ResourceViewColumn](resourceviewcolumn/#constructor_1)(string, int, ResourceToColumnTextConverter) | `ResourceViewColumn` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [ResourceViewColumn](resourceviewcolumn/#constructor_2)(string, int, ResourceToColumnTextConverter, Field) | `ResourceViewColumn` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/resourceviewcolumn/field/) { get; set; } | कॉलम फ़ील्ड। [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | कॉलम का नाम प्राप्त करता है। |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | पाठ की संरेखण प्राप्त करता है या सेट करता है (यह [`HorizontalStringAlignment`](../horizontalstringalignment/) enumeration के मानों में से एक हो सकता है)। |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | कॉलम की कोशिकाओं की उपस्थिति को अनुकूलित करने के लिए उपयोग की जा सकने वाली कॉलबैक प्राप्त करता है या सेट करता है। |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | कॉलम की चौड़ाई प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/resourceviewcolumn/getcolumntext/)(Resource) | वर्तमान संसाधन को कॉलम टेक्स्ट में परिवर्तित करता है। |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


