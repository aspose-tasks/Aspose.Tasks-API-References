---
title: "ResourceViewColumn.ResourceViewColumn"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceViewColumn कंस्ट्रक्टर। ResourceViewColumn क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.visualization/resourceviewcolumn/resourceviewcolumn/
---
## ResourceViewColumn(string, int, ResourceToColumnTextConverter, Field) {#constructor_2}

[`ResourceViewColumn`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public ResourceViewColumn(string name, int width, ResourceToColumnTextConverter converter, 
    Field field)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | स्ट्रिंग | कॉलम का नाम। |
| चौड़ाई | Int32 | कॉलम की चौड़ाई पिक्सेल में। |
| कनवर्टर | ResourceToColumnTextConverter | रिसोर्स डेटा को कॉलम टेक्स्ट में बदलने वाला कनवर्टर। |
| फ़ील्ड | फ़ील्ड | कॉलम फ़ील्ड। |

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

* delegate [ResourceToColumnTextConverter](../../resourcetocolumntextconverter/)
* enum [Field](../../../aspose.tasks/field/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## ResourceViewColumn(string, int, ResourceToColumnTextConverter) {#constructor_1}

[`ResourceViewColumn`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public ResourceViewColumn(string name, int width, ResourceToColumnTextConverter converter)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | स्ट्रिंग | कॉलम का नाम। |
| चौड़ाई | Int32 | कॉलम की चौड़ाई पिक्सेल में। |
| कनवर्टर | ResourceToColumnTextConverter | रिसोर्स डेटा को कॉलम टेक्स्ट में बदलने वाला कनवर्टर। |

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

* delegate [ResourceToColumnTextConverter](../../resourcetocolumntextconverter/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## ResourceViewColumn(int, Field) {#constructor}

[`ResourceViewColumn`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public ResourceViewColumn(int width, Field field)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| चौड़ाई | Int32 | कॉलम की चौड़ाई पिक्सेल में। |
| फ़ील्ड | फ़ील्ड | कॉलम फ़ील्ड। |

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


