---
title: "क्लास TableCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TableCollection क्लास। Table ऑब्जेक्ट्स की सूची शामिल करती है। ICollectionTable इंटरफ़ेस को लागू करती है।"
type: docs
weight: 2330
url: /hi/net/aspose.tasks/tablecollection/
---
## TableCollection class

[`Table`](../table/) ऑब्जेक्ट्स की सूची शामिल करता है। ICollection&lt;Table&gt; इंटरफ़ेस को लागू करता है।

```csharp
public class TableCollection : ICollection<Table>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/tablecollection/count/) { get; } | इस संग्रह में मौजूद तत्वों की संख्या प्राप्त करता है। |
| [IsReadOnly](../../aspose.tasks/tablecollection/isreadonly/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-रीड है या नहीं; अन्यथा, false। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/tablecollection/add/)(Table) | निर्दिष्ट आइटम को इस संग्रह में जोड़ता है। |
| [Clear](../../aspose.tasks/tablecollection/clear/)() | इस संग्रह से सभी आइटम हटाता है। |
| [Contains](../../aspose.tasks/tablecollection/contains/)(Table) | यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false। |
| [CopyTo](../../aspose.tasks/tablecollection/copyto/)(Table[], int) | निर्दिष्ट एरे सूचकांक से शुरू करके इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है। |
| [GetEnumerator](../../aspose.tasks/tablecollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks/tablecollection/remove/)(Table) | इस संग्रह से विशिष्ट वस्तु की पहली घटना को हटाता है। |
| [ToList](../../aspose.tasks/tablecollection/tolist/)() | टेबल संग्रह को [`Table`](../table/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

## उदाहरण

टेबल संग्रहों के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");

Console.WriteLine("Is collection of tables read-only?: " + project.Tables.IsReadOnly);

// टेबल्स पर इटरेट करें
Console.WriteLine("Print tables of " + project.Get(Prj.Name) + " project.");
Console.WriteLine("Table count: " + project.Tables.Count);
foreach (var tbl in project.Tables)
{
    Console.WriteLine("Name: " + tbl.Name);

    Console.WriteLine("Fields:");

    foreach (var field in tbl.TableFields)
    {
        Console.WriteLine("    {0} - '{1}' - {2}", field.Field, field.Title, field.Width);
    }
}

// एक नया टेबल जोड़ें
var tableToAdd = new Table
{
    Name = "New Table",
    ShowInMenu = true
};
project.Tables.Add(tableToAdd);

Console.WriteLine("The collection contains the new table?: " + project.Tables.Contains(tableToAdd));

// संग्रह को दो तरीकों से साफ़ किया जा सकता है
if (deleteOneByOne)
{
    // टेबल्स को एरे में कॉपी करें और उन्हें एक-एक करके हटाएँ
    var tables = new Table[project.Tables.Count];
    project.Tables.CopyTo(tables, 0);
    foreach (var table in tables)
    {
        project.Tables.Remove(table);
    }
}
else
{
    // या टेबल संग्रह को पूरी तरह से साफ़ किया जा सकता है
    project.Tables.Clear();
}

// संग्रह को साधारण टेबल्स की सूची में परिवर्तित किया जा सकता है
List<Table> list = project.Tables.ToList();
foreach (var table in list)
{
    Console.WriteLine("Name: " + table.Name);
}
```

### संबंधित देखें

* class [Table](../table/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


