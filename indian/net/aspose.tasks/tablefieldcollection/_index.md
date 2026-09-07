---
title: "क्लास TableFieldCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TableFieldCollection क्लास। TableField ऑब्जेक्ट्स की एक सूची रखता है। IListTableField इंटरफ़ेस को लागू करता है।"
type: docs
weight: 2350
url: /hi/net/aspose.tasks/tablefieldcollection/
---
## TableFieldCollection class

[`TableField`](../tablefield/) ऑब्जेक्ट्स की एक सूची रखता है। IList&lt;TableField&gt; इंटरफ़ेस को लागू करता है।

```csharp
public class TableFieldCollection : IList<TableField>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/tablefieldcollection/count/) { get; } | इस संग्रह में मौजूद तत्वों की संख्या प्राप्त करता है। |
| [IsReadOnly](../../aspose.tasks/tablefieldcollection/isreadonly/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-रीड है या नहीं; अन्यथा, false। |
| [Item](../../aspose.tasks/tablefieldcollection/item/) { get; set; } | निर्दिष्ट सूचकांक पर तत्व को लौटाता है या सेट करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/tablefieldcollection/add/)(TableField) | निर्दिष्ट आइटम को इस संग्रह में जोड़ता है। |
| [Clear](../../aspose.tasks/tablefieldcollection/clear/)() | इस संग्रह से सभी आइटम हटाता है। |
| [Contains](../../aspose.tasks/tablefieldcollection/contains/)(TableField) | यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false। |
| [CopyTo](../../aspose.tasks/tablefieldcollection/copyto/)(TableField[], int) | निर्दिष्ट एरे सूचकांक से शुरू करके इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है। |
| [GetEnumerator](../../aspose.tasks/tablefieldcollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [IndexOf](../../aspose.tasks/tablefieldcollection/indexof/)(TableField) | इस संग्रह में निर्दिष्ट आइटम का सूचकांक निर्धारित करता है। |
| [Insert](../../aspose.tasks/tablefieldcollection/insert/)(int, TableField) | निर्दिष्ट सूचकांक पर निर्दिष्ट आइटम डालता है। |
| [Remove](../../aspose.tasks/tablefieldcollection/remove/)(TableField) | इस संग्रह से विशिष्ट वस्तु की पहली घटना को हटाता है। |
| [RemoveAt](../../aspose.tasks/tablefieldcollection/removeat/)(int) | निर्दिष्ट सूचकांक पर एक आइटम हटाता है। |

## उदाहरण

टेबल फ़ील्ड संग्रहों के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");

foreach (var tbl in project.Tables)
{
    Console.WriteLine("Table name: " + tbl.Name);
    Console.WriteLine("Is collection of table fields read-only?: " + tbl.TableFields.IsReadOnly);

    // टेबल फ़ील्ड्स पर इटरेट करें
    Console.WriteLine("Print table fields of " + project.Get(Prj.Name) + " project.");
    Console.WriteLine("Table count: " + tbl.TableFields.Count);
    foreach (var fld in tbl.TableFields)
    {
        Console.WriteLine("Field Title: " + fld.Title);
        Console.WriteLine("Field Field: " + fld.Field);
        Console.WriteLine();
    }
}

// एक नया टेबल फ़ील्ड जोड़ें
var table = project.Tables.ToList()[0];
var field = new TableField();
field.Title = "New Table Field";
table.TableFields.Add(field);

var field2 = new TableField();
field2.Title = "New Table Field 2";

// स्थिति में एक नया फ़ील्ड डालें
var idx = table.TableFields.IndexOf(field);
table.TableFields.Insert(idx, field2);

// इंडेक्स एक्सेस का उपयोग करके नया टेबल फ़ील्ड संपादित करें
table.TableFields[idx].WrapHeader = true;

Console.WriteLine("The collection contains the new table field?: " + table.TableFields.Contains(field));

// हाल ही में हम फ़ील्ड को हटा सकते हैं
table.TableFields.RemoveAt(idx);

// संग्रह को दो तरीकों से साफ़ किया जा सकता है
if (deleteOneByOne)
{
    // टेबल फ़ील्ड्स को एरे में कॉपी करें और उन्हें एक-एक करके हटाएँ
    var tableFields = new TableField[table.TableFields.Count];
    table.TableFields.CopyTo(tableFields, 0);
    foreach (var fld in tableFields)
    {
        table.TableFields.Remove(fld);
    }
}
else
{
    // या कोई पूरी तरह से टेबल फ़ील्ड संग्रह को साफ़ कर सकता है
    table.TableFields.Clear();
}
```

### संबंधित देखें

* class [TableField](../tablefield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


