---
title: "Project.Tables"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। Table ऑब्जेक्ट्स की सूची प्राप्त करता है"
type: docs
weight: 900
url: /hi/net/aspose.tasks/project/tables/
---
## Project.Tables property

[`Table`](../../table/) ऑब्जेक्ट्स की सूची प्राप्त करता है।

```csharp
public TableCollection Tables { get; }
```

## उदाहरण

Gantt Chart प्रॉपर्टीज़ को कॉन्फ़िगर करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project5.mpp");
    var task = project.RootTask.Children.Add("New Activity");

    // नया कस्टम एट्रिब्यूट परिभाषित करें
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
    project.ExtendedAttributes.Add(definition);

    // बनाए गए टास्क में कस्टम टेक्स्ट एट्रिब्यूट जोड़ें।
    task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

    // टेबल को कस्टमाइज़ करें टेक्स्ट एट्रिब्यूट फ़ील्ड जोड़कर
    var field = new TableField
    {
        Field = Field.TaskText1,
        Width = 20,
        Title = "Custom attribute",
        AlignTitle = HorizontalStringAlignment.Center,
        AlignData = HorizontalStringAlignment.Center
    };

    var table = project.Tables.ToList()[0];
    table.TableFields.Insert(3, field);

    project.Save(OutDir + @"ConfigureGantChart_out.mpp", new MPPSaveOptions { WriteViewData = true });
}
catch (NotSupportedException ex)
{
    Console.WriteLine(
        ex.Message
        + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http:// Www.aspose.com/purchase/default.aspx.");
}
```

### संबंधित देखें

* class [TableCollection](../../tablecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


