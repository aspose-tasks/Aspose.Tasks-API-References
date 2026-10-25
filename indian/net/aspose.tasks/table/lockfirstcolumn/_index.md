---
title: "Table.LockFirstColumn"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Table प्रॉपर्टी। एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि टेबल की पहली कॉलम लॉक है या संपादन योग्य"
type: docs
weight: 40
url: /hi/net/aspose.tasks/table/lockfirstcolumn/
---
## Table.LockFirstColumn property

टेबल के पहले कॉलम को लॉक किया गया है या संपादन योग्य है, यह दर्शाने वाला मान प्राप्त या सेट करता है।

```csharp
public bool LockFirstColumn { get; set; }
```

## उदाहरण

नया टेबल कैसे परिभाषित करें (व्यूज़ के लिए उपयोग करते हुए) दिखाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");

// संपादन के लिए एक टेबल प्राप्त करें
var table = project.Tables.ToList()[0];
Console.WriteLine("Uid of the table: " + table.Uid);
Console.WriteLine("Name of the table: " + table.Name);
Console.WriteLine("Type of the table: " + table.TableType);

// कुछ गुणों को समायोजित करें
// एक मान सेट करें जो दर्शाता है कि टेबल की हेडर पंक्ति की ऊँचाई समायोजित की जा सकती है या नहीं
table.AdjustHeaderRowHeight = true;

// टेबल की तिथि प्रारूप सेट करें।
table.DateFormat = DateFormat.DateDdMmYyyy;

// एक मान सेट करें जो दर्शाता है कि टेबल का पहला कॉलम लॉक है या संपादनीय
table.LockFirstColumn = true;

// टेबल में पंक्ति की ऊँचाई सेट करें, जहाँ पंक्ति की ऊँचाई टेक्स्ट की पंक्तियों की संख्या होती है
table.RowHeight = 10;

// एक मान सेट करता है जो दर्शाता है कि 'नया कॉलम जोड़ें' इंटरफ़ेस दिखाना है या नहीं
table.ShowAddNewColumn = true;

// एक मान सेट करें जो दर्शाता है कि प्रोजेक्ट रिबन के व्यू टैब पर टेबल्स ड्रॉप-डाउन सूची में टेबल का नाम दिखाता है या नहीं
table.ShowInMenu = true;

// अपडेटेड टेबल को सहेजने देता है
project.Save(OutDir + "WorkWithTable_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


