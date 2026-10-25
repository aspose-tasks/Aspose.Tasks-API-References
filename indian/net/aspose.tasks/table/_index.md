---
title: "क्लास Table"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Table क्लास। प्रोजेक्ट में एक टेबल का प्रतिनिधित्व करता है।"
type: docs
weight: 2320
url: /hi/net/aspose.tasks/table/
---
## Table class

प्रोजेक्ट में एक तालिका को दर्शाता है।

```csharp
public class Table
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Table](table/)() | `Table` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [AdjustHeaderRowHeight](../../aspose.tasks/table/adjustheaderrowheight/) { get; set; } | टेबल की हेडर रो की ऊँचाई को समायोजित किया जा सकता है या नहीं, यह दर्शाने वाला मान प्राप्त या सेट करता है। |
| [DateFormat](../../aspose.tasks/table/dateformat/) { get; set; } | टेबल की डेट फ़ॉर्मेट को प्राप्त या सेट करता है। |
| [LockFirstColumn](../../aspose.tasks/table/lockfirstcolumn/) { get; set; } | टेबल के पहले कॉलम को लॉक किया गया है या संपादन योग्य है, यह दर्शाने वाला मान प्राप्त या सेट करता है। |
| [Name](../../aspose.tasks/table/name/) { get; set; } | टेबल ऑब्जेक्ट का नाम प्राप्त या सेट करता है। |
| [RowHeight](../../aspose.tasks/table/rowheight/) { get; set; } | टेबल में रो की ऊँचाई प्राप्त या सेट करता है, जहाँ रो की ऊँचाई टेक्स्ट की लाइनों की संख्या होती है। |
| [ShowAddNewColumn](../../aspose.tasks/table/showaddnewcolumn/) { get; set; } | 'Add New Column' इंटरफ़ेस दिखाना है या नहीं, यह दर्शाने वाला मान प्राप्त या सेट करता है। MSP 2010 संस्करण और बाद के संस्करणों द्वारा समर्थित। |
| [ShowInMenu](../../aspose.tasks/table/showinmenu/) { get; set; } | प्रोजेक्ट व्यू टैब के रिबन में टेबल्स ड्रॉप-डाउन सूची में टेबल का नाम दिखाता है या नहीं, यह दर्शाने वाला मान प्राप्त या सेट करता है। |
| [TableFields](../../aspose.tasks/table/tablefields/) { get; } | टेबल में फ़ील्ड्स को दर्शाने वाला TableFields कलेक्शन प्राप्त करता है। |
| [TableType](../../aspose.tasks/table/tabletype/) { get; set; } | निर्दिष्ट टेबल के लिए टेबल प्रकार प्राप्त या सेट करता है। |
| [Uid](../../aspose.tasks/table/uid/) { get; } | टेबल का अद्वितीय पहचानकर्ता प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [Equals](../../aspose.tasks/table/equals/)(object) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.tasks/table/gethashcode/)() | इस टेबल के लिए हैश कोड लौटाता है। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


