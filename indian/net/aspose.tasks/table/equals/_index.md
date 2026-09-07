---
title: "Table.Equals"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Table मेथड। एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं"
type: docs
weight: 120
url: /hi/net/aspose.tasks/table/equals/
---
## Table.Equals method

यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public override bool Equals(object obj)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | ऑब्जेक्ट | इस इंस्टेंस के साथ तुलना करने के लिए वस्तु। |

### रिटर्न वैल्यू

**True** if the specified object is a Table that has the same UID value as this instance; otherwise, **false**.

## उदाहरण

टेबल समानता की जाँच कैसे करें दिखाता है।

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// टेबलों की समानता को टेबल के UID के विरुद्ध जाँचा जाता है।
Console.WriteLine("Table 1 UID: " + table1.Uid);
Console.WriteLine("Table 2 UID: " + table2.Uid);
Console.WriteLine("Are tables equal: " + table1.Equals(table2));
```

### संबंधित देखें

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


