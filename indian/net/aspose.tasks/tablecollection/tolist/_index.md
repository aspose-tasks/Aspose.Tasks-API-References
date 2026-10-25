---
title: "TableCollection.ToList"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TableCollection मेथड। टेबल संग्रह को टेबल ऑब्जेक्ट्स की सूची में परिवर्तित करता है।"
type: docs
weight: 90
url: /hi/net/aspose.tasks/tablecollection/tolist/
---
## TableCollection.ToList method

टेबिल संग्रह को [`Table`](../../table/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है।

```csharp
public List<Table> ToList()
```

### रिटर्न वैल्यू

[`Table`](../../table/) ऑब्जेक्ट्स की सामान्य सूची।

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

* class [Table](../../table/)
* class [TableCollection](../)
* namespace [Aspose.Tasks](../../tablecollection/)
* assembly [Aspose.Tasks](../../../)


