---
title: "TableField.TableField"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TableField constructor. TableField क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/tablefield/tablefield/
---
## TableField constructor

[`TableField`](../) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public TableField()
```

## उदाहरण

प्रोजेक्ट टेबल्स को पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// टेबल प्राप्त करें
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// सभी टेबल फ़ील्ड्स की जानकारी प्रदर्शित करें
foreach (var field in table.TableFields)
{
    Console.WriteLine("  Field: " + field.Field);
    Console.WriteLine("  Width: " + field.Width);
    Console.WriteLine("  Title: " + field.Title);
    Console.WriteLine("  Title Alignment: " + field.AlignTitle);
    Console.WriteLine("  Data Alignment: " + field.AlignData);
    Console.WriteLine("  Wrap Header: " + field.WrapHeader);
    Console.WriteLine("  Wrap Text: " + field.WrapText);
    Console.WriteLine();
}
```

### संबंधित देखें

* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


