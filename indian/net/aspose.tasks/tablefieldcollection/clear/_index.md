---
title: "TableFieldCollection.Clear"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TableFieldCollection मेथड। इस संग्रह से सभी आइटम हटाता है"
type: docs
weight: 50
url: /hi/net/aspose.tasks/tablefieldcollection/clear/
---
## TableFieldCollection.Clear method

इस संग्रह से सभी आइटम हटाता है।

```csharp
public void Clear()
```

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

* class [TableFieldCollection](../)
* namespace [Aspose.Tasks](../../tablefieldcollection/)
* assembly [Aspose.Tasks](../../../)


